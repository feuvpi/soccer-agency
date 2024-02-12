<script lang="ts">
	import type { PageData } from './$types';

	export let data: PageData;
</script>

<div class="bg-gray-100 min-h-screen flex items-center justify-center">
	<!-- Imagem de Fundo -->
	<div class="absolute inset-0 z-0">
		<img
			src="https://images.unsplash.com/photo-1599158150601-1417ebbaafdd?q=80&w=1636&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D"
			alt=""
			class="w-full h-full object-cover md:filter-none brightness-50 border-none"
		/>
	</div>

	<!-- Formulário de Registro -->
	<div class="relative z-10 backdrop-blur-md bg-white/30 p-8 rounded-md shadow-lg">
		<h1 class="text-xl font-bold mb-4 text-center">Registre uma conta</h1>
		<form action="#" method="POST">
			<div class="grid grid-cols-2 gap-4">
				<div class="mb-4">
					<label class="block text-gray-700 font-bold mb-2" for="nome">Nome</label>
					<input
						class="appearance-none border rounded-sm py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline w-full"
						id="nome"
						type="text"
						placeholder="Nome"
					/>
				</div>
				<div class="mb-4">
					<label class="block text-gray-700 font-bold mb-2" for="sobrenome">Sobrenome</label>
					<input
						class="appearance-none border rounded-sm py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline w-full"
						id="sobrenome"
						type="text"
						placeholder="Sobrenome"
					/>
				</div>
			</div>
			<div class="mb-4">
				<label class="block text-gray-700 font-bold mb-2" for="email">Email</label>
				<input
					class="appearance-none border rounded-sm py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline w-full"
					id="email"
					type="email"
					placeholder="Email"
				/>
			</div>
			<div class="mb-4">
				<label class="block text-gray-700 font-bold mb-2" for="senha">Senha</label>
				<input
					class="appearance-none border rounded-sm py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline w-full"
					id="senha"
					type="password"
					placeholder="Senha"
				/>
			</div>
			<div class="mb-4">
				<label class="block text-gray-700 font-bold mb-2" for="confirmar-senha"
					>Confirmar Senha</label
				>
				<input
					class="appearance-none border rounded-sm py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline w-full"
					id="confirmar-senha"
					type="password"
					placeholder="Confirmar Senha"
				/>
			</div>

			<div class="mt-6 mb-2 justify-center flex">
				<button
					class="rounded-sm text-center items-center justify-center flex flex-no-wrap border-2 border-black bg-yellow-500 py-2 px-4 mb-4 w-full w-2/4"
				>
					<span>Registrar</span>
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
			</div>

			<button
				class="justify-center flex items-center bg-white border-gray-300 rounded-sm shadow-md px-6 py-2 text-sm font-medium text-gray-800 hover:bg-gray-200 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-gray-500 w-full"
			>
				<svg
					class="h-6 w-6 mr-2"
					xmlns="http://www.w3.org/2000/svg"
					xmlns:xlink="http://www.w3.org/1999/xlink"
					width="800px"
					height="800px"
					viewBox="-0.5 0 48 48"
					version="1.1"
				>
					<title>Google-color</title> <desc>Created with Sketch.</desc> <defs> </defs>
					<g id="Icons" stroke="none" stroke-width="1" fill="none" fill-rule="evenodd">
						<g id="Color-" transform="translate(-401.000000, -860.000000)">
							<g id="Google" transform="translate(401.000000, 860.000000)">
								<path
									d="M9.82727273,24 C9.82727273,22.4757333 10.0804318,21.0144 10.5322727,19.6437333 L2.62345455,13.6042667 C1.08206818,16.7338667 0.213636364,20.2602667 0.213636364,24 C0.213636364,27.7365333 1.081,31.2608 2.62025,34.3882667 L10.5247955,28.3370667 C10.0772273,26.9728 9.82727273,25.5168 9.82727273,24"
									id="Fill-1"
									fill="#FBBC05"
								>
								</path>
								<path
									d="M23.7136364,10.1333333 C27.025,10.1333333 30.0159091,11.3066667 32.3659091,13.2266667 L39.2022727,6.4 C35.0363636,2.77333333 29.6954545,0.533333333 23.7136364,0.533333333 C14.4268636,0.533333333 6.44540909,5.84426667 2.62345455,13.6042667 L10.5322727,19.6437333 C12.3545909,14.112 17.5491591,10.1333333 23.7136364,10.1333333"
									id="Fill-2"
									fill="#EB4335"
								>
								</path>
								<path
									d="M23.7136364,37.8666667 C17.5491591,37.8666667 12.3545909,33.888 10.5322727,28.3562667 L2.62345455,34.3946667 C6.44540909,42.1557333 14.4268636,47.4666667 23.7136364,47.4666667 C29.4455,47.4666667 34.9177955,45.4314667 39.0249545,41.6181333 L31.5177727,35.8144 C29.3995682,37.1488 26.7323182,37.8666667 23.7136364,37.8666667"
									id="Fill-3"
									fill="#34A853"
								>
								</path>
								<path
									d="M46.1454545,24 C46.1454545,22.6133333 45.9318182,21.12 45.6113636,19.7333333 L23.7136364,19.7333333 L23.7136364,28.8 L36.3181818,28.8 C35.6879545,31.8912 33.9724545,34.2677333 31.5177727,35.8144 L39.0249545,41.6181333 C43.3393409,37.6138667 46.1454545,31.6490667 46.1454545,24"
									id="Fill-4"
									fill="#4285F4"
								>
								</path>
							</g>
						</g>
					</g>
				</svg>
				<span>Continuar com o Google</span>
			</button>
		</form>
	</div>
</div>
