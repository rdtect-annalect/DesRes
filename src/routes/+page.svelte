<script>
	import Slides from '$lib/deck/slides.svelte';
	let a = $state(4)
let b= 0;
	function increment() {
		a += 1
	}

</script>

<svelte:head>
	<title>Presentation</title>
</svelte:head>

<p class="text-center text-white text-4xl font-bold">Presentation</p>
<Slides />
<div class =" flex justify-center ">

	<button on:click={increment} class=" bg-white p-4 before:border-blue-500 border-solid border-t-2 hover:border-green-200 focus:bg-yellow-100"> click for {a} </button>
</div>


