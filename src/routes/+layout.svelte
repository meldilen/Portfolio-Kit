<script>
	import Header from './Header.svelte';
	import Fouter from './Fouter.svelte';
</script>

<div class="app">
	<Header />

	<main>
		<slot />
	</main>

</div>

<Fouter />

<style>
	.app {
		display: flex;
		flex-direction: column;
		min-height: 90.5vh;
	}
</style>
