<script lang="ts">
  	import Calculadora from "./components/Calculadora.svelte";
</script>

<main>
		<Calculadora />
</main>

<style>


	:global(body){
		background-color: #161616;
	}

	:root{
		--cor-fundo: #555;
	}

	main {
		display: flex;
		align-items: center;
		justify-content: center;
		height: 100vh;
	}
	
</style>