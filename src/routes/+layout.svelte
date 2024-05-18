<script lang="ts">
	import '../app.css';
	import Footer from '$lib/components/common/Footer.svelte';
	import Navbar from '$lib/components/common/Navbar.svelte';
	import Sidebar from '$lib/components/common/Sidebar.svelte';

	let open: boolean = false;
</script>

<div class="lg:hidden">
	<Sidebar bind:open />
</div>
<div class="w-full z-50 fixed">
	<Navbar bind:open />
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
