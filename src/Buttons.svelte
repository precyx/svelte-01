<script>
import Button from "./Button.svelte";

var array = new Array(10).fill(0);


const randomColor = () => {
	var letters = '0123456789ABCDEF';
  var color = '#';
  for (var i = 0; i < 6; i++) {
    color += letters[Math.floor(Math.random() * 16)];
  }
  return color; 
}

</script>

<style>
</style>

<div>
{#each array as el, i}
	<Button value={"Button " + i} color={randomColor()} />
{/each}
</div>

