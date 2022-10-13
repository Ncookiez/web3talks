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
		/* border: 1em solid var(--primary-color); */
		overflow: hidden;
	}

</style>