<script>

import {a} from "./blob";


console.log("dasasdas")

	let pokemons = [];

  async function getData(){
    let response = await fetch("https://api.kikoweb.ch/lib/pokedex/pokedex.php");
    pokemons = await response.json()
		console.log(pokemons);
  }
  getData()
</script>

<style>
    h1 {
        color: purple;
    }
</style>

<h1>Hello {name}!</h1>

{#await pokemons}
	<p>...waiting</p>
{:then pokemons}
	<p>The number is {pokemons.length}</p>
{:catch error}
	<p style="color: red">{error.message}</p>
{/await}


{#each pokemons as pokemon}
<div>{pokemon.ename}</div>
{/each}


