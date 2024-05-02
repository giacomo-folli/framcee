<script lang="ts">
	import Hamburger from './Hamburger.svelte';

	export let open: boolean = false;
</script>

<header class="p-4 flex items-center justify-between">
	<a href="/">
		<img class="h-10 w-10" src="/logo.png" alt="logo" />
	</a>

	<Hamburger bind:open />
</header>
