<script>
	import '../app.css'
	import '@fontsource/spartan/400.css'
	import '@fontsource/spartan/500.css'
	import '@fontsource/spartan/600.css'
	import '@fontsource/spartan/700.css'
	import Navbar from '$lib/components/Navbar.svelte'
</script>

<div class="text-black">
	<Navbar />
	<slot />
</div>
