<script lang="ts">
    import Joke from "./joke.svelte";
    import Bio from "./bio.svelte";
</script>

<svelte:head>
	<title>Home</title>
	<meta name="description" content="Svelte demo app" />
</svelte:head>

<main>
	<Bio/>
	<Joke/>
</main>

<style>
	*{
	  margin: 0; 
	  padding:0; 
	  background-image: url(https://phonoteka.org/uploads/posts/2022-02/1643900978_1-phonoteka-org-p-serii-akvarelnii-fon-1.jpg);
	  background-size: cover;
	}
</style>


