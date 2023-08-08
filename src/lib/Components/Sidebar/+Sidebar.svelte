<script>
	export let open = false;
	export let data
	const {products} = data;
	console.log(data)
</script>

<aside class="absolute w-full h-full bg-gray-200 border-r-2 shadow-lg" class:open>
	<nav class="p-12 text-xl">
		{#each products as product}
			<h3>product.title</h3>
		{/each}
	</nav>
</aside>

<style>
	aside {
		left: -100%;
		transition: left 0.3s ease-in-out
	}
	
	.open {
		left: 0
	}
</style>