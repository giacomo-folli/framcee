<script lang="ts">
	export let open: boolean = false;
</script>

<div class="py-2 text-black relative bg-opacity-45 backdrop-blur-lg">
	<nav>
		<div class="w-full px-4">
			<div class="w-full flex items-center justify-between">
				<a class="font-black text-3xl min-w-[33%] overflow-hidden pl-2" href="/">
					<img src="/2.png" alt="logo-navbar" class="h-[60px]" />
				</a>
				<button
					class="block lg:hidden cursor-pointer h-10 z-20"
					type="button"
					id="hamburger"
					on:click={() => (open = !open)}
				>
					<div class="h-0.5 w-7 bg-black -translate-y-2"></div>
					<div class="h-0.5 w-7 bg-black"></div>
					<div class="h-0.5 w-7 bg-black translate-y-2"></div>
				</button>
				<div
					class="grow flex flex-col lg:flex-row justify-center lg:justify-between items-center text-3xl gap-6 lg:text-base lg:gap-2 absolute h-screen w-screen top-0 left-full lg:left-0 lg:relative lg:h-auto lg:w-auto bg-white dark:bg-[#0b1727] lg:bg-transparent"
					id="navbar"
				>
					<ul class="w-full flex justify-center">
						<li class="">
							<a class="px-4" href="/classi">Classi</a>
						</li>
						<li class="">
							<a class="px-4" href="/personal">Personal</a>
						</li>
						<li class="">
							<a class="px-4" href="/about">About</a>
						</li>
					</ul>
					<ul class="min-w-[45%] flex justify-end mb-2 lg:mb-0">
						<li>
							<button
								class="border border-black hover:bg-black hover:text-white rounded-lg px-4 py-1.5"
							>
								Prossime sessioni
							</button>
						</li>
					</ul>
				</div>
			</div>
		</div>
	</nav>
</div>
