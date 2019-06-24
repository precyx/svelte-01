<script>
	import Test from "./Test.svelte";
	import Button from "./Button.svelte";
	import Buttons from "./Buttons.svelte";

	export let name;


</script>

<style>
	h1 {
		color: purple;
	}
</style>

<h1>Hello {name} tesssst!</h1>

<Button value="test" />

<Buttons></Buttons>

<Test></Test>
