<script>
	import About from '$lib/components/About.svelte';
	import HappyClients from '$lib/components/HappyClients.svelte';
	import Header from '$lib/components/Header.svelte';
	import JoinUs from '$lib/components/JoinUs.svelte';
	import Products from '$lib/components/Products.svelte';
	import Sponsers from '$lib/components/Sponsers.svelte';
	import Why from '$lib/components/Why.svelte';
</script>

<!-- YOU CAN DELETE EVERYTHING IN THIS PAGE -->

<div class="flex flex-col items-center justify-center mx-auto">
	<Header />
	<Sponsers />
	<About />
	<Why />
	<Products />
	<HappyClients />
	<JoinUs />
</div>
