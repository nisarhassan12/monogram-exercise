<script>
	import Container from './container.svelte';
</script>

<style lang="postcss">
	div {
		@apply border-r border-dashed border-[#3f3f3f];
	}

	div:first-child {
		@apply border-l border-dashed border-[#3f3f3f]; 
	}
</style>

<Container class="grid grid-cols-4 h-full w-full absolute top-0 right-0 left-0 bottom-0 -z-10">
	<div></div>
	<div></div>
	<div></div>
	<div></div>
</Container>
