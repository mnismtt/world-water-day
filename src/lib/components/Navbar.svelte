<script>
	import { fly } from 'svelte/transition'

	const navLinks = ['Services', 'About', 'Contact']
	let isShow = false
</script>

<nav class="fixed top-0 z-10 w-full py-8">
	<div
		class="flex items-center justify-between px-8 mx-auto space-x-32 lg:justify-start lg:px-0 lg:max-w-5xl xl:max-w-7xl"
	>
		<div class="flex items-center space-x-1 cursor-pointer">
			<img src="/images/logo.png" alt="Logo" width={38} height={38} />
			<h1 class="text-2xl font-bold transition duration-300 hover:opacity-75">waterworks</h1>
		</div>

		<div class="hidden space-x-16 md:flex">
			{#each navLinks as navLink}
				<a href="/" class="font-medium transition duration-300 hover:text-gray-600">{navLink}</a>
			{/each}
		</div>
		<div class="block md:hidden">
			<button on:click={() => (isShow = true)}>
				<img src="/images/hamburger.svg" alt="Hamburger" width={24} height={24} />
			</button>
		</div>
	</div>
</nav>

{#if isShow}
	<div class="fixed top-0 left-0 z-20 w-screen h-screen bg-black opacity-90" transition:fly>
		<button class="fixed top-10 right-10" on:click={() => (isShow = false)}>
			<img src="/images/close.svg" alt="Close" width={36} height={36} />
		</button>
		<div class="z-30 flex flex-col items-center justify-center w-full h-full space-y-12">
			{#each navLinks as navLink}
				<a
					href="/"
					class="text-4xl font-bold text-white transition duration-300 hover:text-gray-600"
					>{navLink}</a
				>
			{/each}
		</div>
	</div>
{/if}
