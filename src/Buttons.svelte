<script>
import Button from "./Button.svelte";

var array = new Array(10).fill(0);

</script>

<style>
</style>

<div>
{#each array as el, i}
	<Button value={"Button " + i} />
{/each}
</div>

