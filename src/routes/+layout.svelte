<script lang="ts">

	// Imports:
	import '../app.css';
	
</script>

<!-- #################################################################################################### -->

<!-- App Content -->
<main><slot /></main>

<!-- #################################################################################################### -->

<style>

	main {
		display: flex;
		flex-direction: column;
		min-height: 100vh;
		overflow-x: hidden;
	}

</style>