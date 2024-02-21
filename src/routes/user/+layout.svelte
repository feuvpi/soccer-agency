<script>
	import 'tailwindcss/tailwind.css';
	import { page } from '$app/stores';
	import { browser } from '$app/environment';

	import TopBar from '$lib/components/Topbar.svelte';
	import Overlay from '$lib/components/Overlay.svelte';
	import Sidebar from '$lib/components/Sidebar/Sidebar.svelte';
	import { closeSidebar, sidebarOpen } from '../../lib/utils/store';

	const style = {
		container: `bg-gray-100 h-screen overflow-hidden relative`,
		main: `h-screen overflow-auto pb-36 pt-4 px-2 md:pb-8 lg:px-4`,
		mainContainer: `flex flex-col h-screen pl-0 w-full lg:pl-24 lg:space-y-4`
	};

	if (browser) {
		page.subscribe(() => {
			// close Sidebar on route changes when sidebar is open
			if ($sidebarOpen) {
				closeSidebar();
			}
		});
	}
</script>

<div
	class={style.container}
	style="background-image: url('https://images.unsplash.com/photo-1561457909-cbbf7d732ee6?q=80&w=2127&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D'); background-size: cover; background-color: rgba(255, 255, 255, 0.5);"
>
	<div class="flex items-start">
		<Overlay />
		<Sidebar mobileOrientation="end" />
		<div class={style.mainContainer}>
			<TopBar />
			<main class={style.main}>
				<slot />
			</main>
		</div>
	</div>
</div>
