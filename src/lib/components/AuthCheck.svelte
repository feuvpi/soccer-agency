<script lang="ts">
	//import { user } from '$lib/firebase';
</script>

<!-- {#if $user} -->
<slot />
<!-- {:else} -->
// -- redirect to landing page
<!-- <p class="text-error my-10">
		Please, sign in to view this page.
		<a class="btn btn-primary" href="/login">Sign in</a>
	</p> -->
<!-- {/if} -->
