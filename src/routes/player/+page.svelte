<!-- <script lang="ts">
	import type { PageData } from './$types';

	export let data: PageData;
</script> -->

<script>
// @ts-nocheck

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

<div class="relative  mx-auto px-4 py-8 bg-gradient-to-bl from-lime-400 via-emerald-500 to-green-600">
    <!-- <div class="absolute w-full bottom-0">
        <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1440 320">
            <path fill="#00cba9" fill-opacity="1" d="M0,32L60,69.3C120,107,240,181,360,181.3C480,181,600,107,720,101.3C840,96,960,160,1080,202.7C1200,245,1320,267,1380,277.3L1440,288L1440,320L1380,320C1320,320,1200,320,1080,320C960,320,840,320,720,320C600,320,480,320,360,320C240,320,120,320,60,320L0,320Z"></path>
        </svg>
    </div> -->


<!-- <div class="container mx-auto px-4 py-8 border-indigo-700 border-2"> -->
	<div class="flex flex-col md:flex-row bg-transparent">
		<div class="md:w-1/2 border-red-300 border-2 p-2">
			<img
				src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQWaG_RSck-_oVJNSOCX9b3_Eiwd95OmSRQ4kUuUNf6RQ&s"
				alt="Imagem do Jogador"
				class="mx-auto w-auto h-full md:w-auto mt-6"
				style="max-width: 300px; height: 100vh;"
			/>
		</div>
	
		
		<div class="md:w-1/2 bg-transparent md:pl-8 border-red-300 border-2 p-2">
	
			<h1 class="text-2xl font-bold py-8">{player.name}</h1>

			<div class="py-10 md:py-8">
				<div class="container max-w-screen-xl mx-auto px-4">
					<div class="grid items-center grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
						<div class="bg-gray-50 px-8 py-10 rounded-md shadow-md">
							<div class="w-20 py-6 flex justify-center bg-gray-100 rounded-md mb-4">
								<i data-feather="coffee"></i>
							</div>

							<h4 class="font-medium text-gray-700 text-lg mb-4">POSIÇÃO</h4>

							<p class="font-normal text-gray-500 text-md">LATERAL ESQUERDO</p>
						</div>

						<div class="bg-gray-100 px-8 py-10 rounded-md shadow-md">
							<div class="w-20 py-6 flex justify-center bg-gray-100 rounded-md mb-4">
								<i data-feather="activity"></i>
							</div>

							<h4 class="font-medium text-gray-700 text-lg mb-4">IDADE</h4>

							<p class="font-normal text-gray-500 text-md">23</p>
						</div>

						<div class="bg-gray-50 px-8 py-10 rounded-md shadow-md">
							<div class="w-20 py-6 flex justify-center bg-gray-100 rounded-md mb-4">
								<i data-feather="codesandbox"></i>
							</div>

							<h4 class="font-medium text-gray-700 text-lg mb-4">ALTURA</h4>

							<p class="font-normal text-gray-500 text-md">1,74M</p>
						</div>

						<div class="bg-gray-50 px-8 py-10 rounded-md shadow-md">
							<div class="w-20 py-6 flex justify-center bg-gray-100 rounded-md mb-4">
								<i data-feather="coffee"></i>
							</div>

							<h4 class="font-medium text-gray-700 text-lg mb-4">PESO</h4>

							<p class="font-normal text-gray-500 text-md">75KG</p>
						</div>

						<div class="bg-gray-50 px-8 py-10 rounded-md shadow-md">
							<div class="w-20 py-6 flex justify-center bg-gray-100 rounded-md mb-4">
								<i data-feather="coffee"></i>
							</div>

							<h4 class="font-medium text-gray-700 text-lg mb-4">PÉ PREFERIDO</h4>

							<p class="font-normal text-gray-500 text-md">DIREITO</p>
						</div>

						<div class="bg-gray-50 px-8 py-10 rounded-md shadow-md">
							<div class="w-20 py-6 flex justify-center bg-gray-100 rounded-md mb-4">
								<i data-feather="coffee"></i>
							</div>

							<h4 class="font-medium text-gray-700 text-lg mb-4">GOL MARCADOS</h4>

							<p class="font-normal text-gray-500 text-md">32</p>
						</div>

						<div class="bg-gray-50 px-8 py-10 rounded-md shadow-md">
							<div class="w-20 py-6 flex justify-center bg-gray-100 rounded-md mb-4">
								<i data-feather="coffee"></i>
							</div>

							<h4 class="font-medium text-gray-700 text-lg mb-4">TIMES ATUAL</h4>

							<p class="font-normal text-gray-500 text-md">BAHIA DE FEIRA</p>
						</div>

						<div class="bg-gray-50 px-8 py-10 rounded-md shadow-md">
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
	

	
	<!-- </div> -->

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

	<div style="overflow: hidden;">
		<svg
		  preserveAspectRatio="none"
		  viewBox="0 0 1200 120"
		  xmlns="http://www.w3.org/2000/svg"
		  style={{ fill: '#64ffa1', width: '400%', height: 445, transform: 'rotate(180deg) scaleX(-1)' }}
		>
		  <path
		  d="M0 0v46.29c47.79 22.2 103.59 32.17 158 28 70.36-5.37 136.33-33.31 206.8-37.5 73.84-4.36 147.54 16.88 218.2 35.26 69.27 18 138.3 24.88 209.4 13.08 36.15-6 69.85-17.84 104.45-29.34C989.49 25 1113-14.29 1200 52.47V0z"
		  opacity=".25"
		/>
		  <path
			d="M0 0v15.81c13 21.11 27.64 41.05 47.69 56.24C99.41 111.27 165 111 224.58 91.58c31.15-10.15 60.09-26.07 89.67-39.8 40.92-19 84.73-46 130.83-49.67 36.26-2.85 70.9 9.42 98.6 31.56 31.77 25.39 62.32 62 103.63 73 40.44 10.79 81.35-6.69 119.13-24.28s75.16-39 116.92-43.05c59.73-5.85 113.28 22.88 168.9 38.84 30.2 8.66 59 6.17 87.09-7.5 22.43-10.89 48-26.93 60.65-49.24V0z"
			opacity=".5"
		  />
		  <path d="M0 0v5.63C149.93 59 314.09 71.32 475.83 42.57c43-7.64 84.23-20.12 127.61-26.46 59-8.63 112.48 12.24 165.56 35.4C827.93 77.22 886 95.24 951.2 90c86.53-7 172.46-45.71 248.8-84.81V0z" />
		</svg>
	  </div>
</div>

<style>
	/* Add custom styles here */
</style>
