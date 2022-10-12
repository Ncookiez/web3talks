<script>

	// Imports:
	import Nav from '$lib/Nav.svelte';
	import '../app.css';
	
</script>

<!-- #################################################################################################### -->

<!-- Navbar -->
<Nav />

<!-- App Content -->
<main><slot /></main>

<!-- #################################################################################################### -->

<style>

	main {
		display: flex;
		flex-direction: column;
		padding: 1em;
		overflow-x: hidden;
	}

</style>