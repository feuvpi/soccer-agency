<script lang="ts">
	import type { PageData } from './$types';

	export let data: PageData;
</script>

<div class="bg-gray-100 min-h-screen flex items-center justify-center">
	<!-- Imagem de Fundo -->
	<div class="absolute inset-0 z-0">
		<img
			src="https://images.unsplash.com/photo-1510051640316-cee39563ddab?q=80&w=1740&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D"
			alt=""
			class="w-full h-full object-cover md:filter-none brightness-50 border-none"
		/>
	</div>

	<!-- Formulário de Contato -->
	<div class="relative w-auto md:w-1/4 z-10 backdrop-blur-md bg-white/30 p-8 rounded-md shadow-lg">
		<h1 class="text-xl font-bold mb-4 text-center">Entre em Contato</h1>
		<form action="#" method="POST">
			<div class="mb-4">
				<label class="block text-gray-700 font-bold mb-2" for="nome">Nome</label>
				<input
					class="appearance-none border rounded-md py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline w-full"
					id="nome"
					type="text"
					placeholder="Nome"
				/>
			</div>
			<div class="mb-4">
				<label class="block text-gray-700 font-bold mb-2" for="email">Email</label>
				<input
					class="appearance-none border rounded-md py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline w-full"
					id="email"
					type="email"
					placeholder="Email"
				/>
			</div>
			<div class="mb-4">
				<label class="block text-gray-700 font-bold mb-2" for="mensagem">Mensagem</label>
				<textarea
					class="resize-none border rounded-md py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline w-full"
					id="mensagem"
					placeholder="Digite sua mensagem aqui..."
					rows="4"
				></textarea>
			</div>
			<button class="flex flex-no-wrap border-2 border-black bg-yellow-500 py-2 px-4 mb-4 w-full">
				<span>Enviar Mensagem</span>
				<span>
					<svg
						xmlns="http://www.w3.org/2000/svg"
						width="24"
						height="24"
						viewBox="0 0 24 24"
						fill="none"
						stroke="currentColor"
						stroke-width="2"
						stroke-linecap="round"
						stroke-linejoin="round"
						class="ml-2 w-6 h-6"
						><line x1="5" y1="12" x2="19" y2="12"></line><polyline points="12 5 19 12 12 19"
						></polyline></svg
					>
				</span>
			</button>
		</form>
	</div>
</div>
