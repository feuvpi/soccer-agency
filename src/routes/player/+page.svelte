<!-- <script lang="ts">
	import type { PageData } from './$types';

	export let data: PageData;
</script> -->

<script>
	import { onMount } from 'svelte';
	let player = {
		name: 'Player Name',
		age: 25,
		weight: '75 kg',
		height: '180 cm',
		preferredFoot: 'Right',
		mainPosition: 'Forward',
		secondaryPosition: 'Midfielder',
		goals: 50,
		actualTeam: 'Current Team',
		teamsDefended: ['Team A', 'Team B']
	};

	let videos = ['video1.mp4', 'video2.mp4', 'video3.mp4'];

	onMount(() => {
		// Fetch player data and videos here
	});
</script>

<div class="container mx-auto px-4 py-8">
	<div class="flex flex-col md:flex-row">
		<div class="md:w-1/2 border-indigo-300 border-2 p-2">
			<img
				src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQWaG_RSck-_oVJNSOCX9b3_Eiwd95OmSRQ4kUuUNf6RQ&s"
				alt="Imagem do Jogador"
				class="mx-auto w-auto h-full md:w-auto mt-6"
				style="max-width: 300px; height: 100vh;"
			/>
		</div>
		<div class="md:w-1/2 md:pl-8 border-red-300 border-2 p-2">
			<h1 class="text-2xl font-bold py-8">{player.name}</h1>

			<div class="py-10 md:py-8">
				<div class="container max-w-screen-xl mx-auto px-4">
					<div class="grid items-center grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
						<div class="bg-gray-50 px-8 py-10 rounded-md">
							<div class="w-20 py-6 flex justify-center bg-gray-100 rounded-md mb-4">
								<i data-feather="coffee"></i>
							</div>

							<h4 class="font-medium text-gray-700 text-lg mb-4">POSIÇÃO</h4>

							<p class="font-normal text-gray-500 text-md">LATERAL ESQUERDO</p>
						</div>

						<div class="bg-gray-100 px-8 py-10 rounded-md">
							<div class="w-20 py-6 flex justify-center bg-gray-100 rounded-md mb-4">
								<i data-feather="activity"></i>
							</div>

							<h4 class="font-medium text-gray-700 text-lg mb-4">IDADE</h4>

							<p class="font-normal text-gray-500 text-md">23</p>
						</div>

						<div class="bg-gray-50 px-8 py-10 rounded-md">
							<div class="w-20 py-6 flex justify-center bg-gray-100 rounded-md mb-4">
								<i data-feather="codesandbox"></i>
							</div>

							<h4 class="font-medium text-gray-700 text-lg mb-4">ALTURA</h4>

							<p class="font-normal text-gray-500 text-md">1,74M</p>
						</div>

						<div class="bg-gray-50 px-8 py-10 rounded-md">
							<div class="w-20 py-6 flex justify-center bg-gray-100 rounded-md mb-4">
								<i data-feather="coffee"></i>
							</div>

							<h4 class="font-medium text-gray-700 text-lg mb-4">PESO</h4>

							<p class="font-normal text-gray-500 text-md">75KG</p>
						</div>

						<div class="bg-gray-50 px-8 py-10 rounded-md">
							<div class="w-20 py-6 flex justify-center bg-gray-100 rounded-md mb-4">
								<i data-feather="coffee"></i>
							</div>

							<h4 class="font-medium text-gray-700 text-lg mb-4">PÉ PREFERIDO</h4>

							<p class="font-normal text-gray-500 text-md">DIREITO</p>
						</div>

						<div class="bg-gray-50 px-8 py-10 rounded-md">
							<div class="w-20 py-6 flex justify-center bg-gray-100 rounded-md mb-4">
								<i data-feather="coffee"></i>
							</div>

							<h4 class="font-medium text-gray-700 text-lg mb-4">GOL MARCADOS</h4>

							<p class="font-normal text-gray-500 text-md">32</p>
						</div>

						<div class="bg-gray-50 px-8 py-10 rounded-md">
							<div class="w-20 py-6 flex justify-center bg-gray-100 rounded-md mb-4">
								<i data-feather="coffee"></i>
							</div>

							<h4 class="font-medium text-gray-700 text-lg mb-4">TIMES ATUAL</h4>

							<p class="font-normal text-gray-500 text-md">BAHIA DE FEIRA</p>
						</div>

						<div class="bg-gray-50 px-8 py-10 rounded-md">
							<div class="w-20 py-6 flex justify-center bg-gray-100 rounded-md mb-4">
								<i data-feather="coffee"></i>
							</div>

							<h4 class="font-medium text-gray-700 text-lg mb-4">TIMES DEFENDIDOS</h4>

							<p class="font-normal text-gray-500 text-md">BAHIA DE FEIRA, VITORIA</p>
						</div>
					</div>
				</div>
			</div>

			<!-- <ul>
				<li><strong>Age:</strong> {player.age}</li>
				<li><strong>Weight:</strong> {player.weight}</li>
				<li><strong>Height:</strong> {player.height}</li>
				<li><strong>Preferred Foot:</strong> {player.preferredFoot}</li>
				<li><strong>Main Position:</strong> {player.mainPosition}</li>
				<li><strong>Secondary Position:</strong> {player.secondaryPosition}</li>
				<li><strong>Number of Goals:</strong> {player.goals}</li>
				<li><strong>Actual Team:</strong> {player.actualTeam}</li>
				<li><strong>Teams Defended:</strong> {player.teamsDefended.join(', ')}</li>
			</ul> -->
		</div>
	</div>

	<div class="mt-8">
		<h2 class="text-xl font-bold mb-4">Videos</h2>
		<div class="grid grid-cols-1 md:grid-cols-3 gap-4">
			<!-- {#each videos as video}
				<div class="border border-gray-200 rounded overflow-hidden">
					<video controls class="w-full">
						<source src={video} type="video/mp4" />
						Your browser does not support the video tag.
					</video>
				</div>
			{/each} -->
		</div>
	</div>

	<div class="mt-8">
		<h2 class="text-xl font-bold mb-4">Contact</h2>
		<p>Contact information of the player's agent goes here.</p>
	</div>
</div>

<style>
	/* Add custom styles here */
</style>
