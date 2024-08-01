<script>
	export let error;
	export let status;
</script>

<main class="error-container bg-blue-950 text-slate-300 p-4">
	<div class="max-w-screen-xl mx-auto px-4 sm:px-6 lg:px-8">
		<div class="flex flex-col items-center">
			<svg
				class="w-16 h-16 text-indigo-600 mb-4"
				fill="none"
				stroke="currentColor"
				viewBox="0 0 24 24"
				xmlns="http://www.w3.org/2000/svg"
			>
				<path
					stroke-linecap="round"
					stroke-linejoin="round"
					stroke-width="2"
					d="M13 16h-1v-4h-1m-1-4h.01M12 2a10 10 0 100 20 10 10 0 000-20z"
				></path>
			</svg>
			<h1 class="text-4xl font-bold mb-2">Sorry, this page doesn't exist.</h1>
			<p class="text-lg mb-4">
				The page you are looking for might have been removed, had its name changed, or is
				temporarily unavailable.
			</p>
			<a href="/" class="text-blue-500 hover:text-blue-700">Go to Homepage</a>
		</div>
	</div>
</main>

<style>
	.error-container {
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
		height: 100vh;
		text-align: center;
	}
</style>
