<script lang="ts">
	import '../app.css';
	import Footer from '$lib/components/common/Footer.svelte';
	import Navbar from '$lib/components/common/Navbar.svelte';

	let open: boolean = false;
</script>

<div class="w-full z-50 fixed">
	<Navbar />
</div>

<div class:open>
	<slot />
	<Footer />
</div>

<style>
	.open {
		z-index: -1;
		position: fixed;
	}
</style>
