<script lang="ts">
	export let open: boolean = false;
</script>

<div class="absolute z-20">
	<aside class="fixed w-full h-full bg-white" class:open>
		<nav class="mt-10 p-12 text-4xl flex flex-col gap-3">
			<a class="block" on:click={() => open = false} href="/">Home</a>
			<a class="block" on:click={() => open = false} href="/classi">Classi</a>
			<a class="block" on:click={() => open = false} href="/personal">Personal</a>
			<a class="block" on:click={() => open = false} href="/about">About</a>
		</nav>
		
		<div class="w-full absolute bottom-12 flex justify-center items-center gap-6">
			<a href="https://www.instagram.com/francescobernini7/">
				<a class="text-3xl" href="https://www.instagram.com/francescobernini7/">
					<span class="mdi mdi-instagram"></span>
				</a>
			</a>
			<a class="text-3xl" href="mailto:giacomofolli01@gmail.com">
				<span class="mdi mdi-email-outline"></span>
			</a>
		</div>
	</aside>
</div>

<style>
	aside {
		left: -100%;
		transition: left 0.3s ease-in-out;
	}

	.open {
		display: block;
		left: 0;
	}
</style>
