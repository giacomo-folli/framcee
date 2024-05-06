<script lang="ts">
	import Hamburger from './Hamburger.svelte';

	export let open: boolean = false;
</script>

<header
	class="{open ? 'fixed' : 'absolute'} w-full p-4 flex flex-end items-center justify-between z-50"
>
	<a href="/">
		<img class="h-10 w-10" src="/logo.png" alt="logo" />
	</a>

	<Hamburger bind:open />
</header>
