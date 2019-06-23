<script>

export let value;
export let isOn = false;
$: status = isOn ? "on" : "off";

</script>


<style>
	.button {
		border:1px solid grey;
		padding:8px;
		display:inline-flex;
		cursor: pointer;
		border-radius:8px;
		user-select:none;
		margin-right:10px;
		margin-bottom:10px;
	}
</style>


<div class="button" on:click={() => {isOn = !isOn}}>
	{value} {status}
</div>