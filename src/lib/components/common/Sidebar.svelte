<script lang="ts">
	export let open: boolean = false;
</script>

<aside class="absolute w-full h-full bg-white z-1" class:open>
	<nav class="p-12 text-4xl flex flex-col gap-3">
		<a class="block" href="/">Home</a>
		<a class="block" href="/classi">Classi</a>
		<a class="block" href="/personal">Personal</a>
		<a class="block" href="/about">About</a>
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
