<script lang="ts">
	import Lines from './lines.svelte';
	import SquigglyDark from './squiggly-dark.svelte';
	let clazz = '';
	export { clazz as class };
	export let renderSquiggly: boolean = false;
</script>

<div class="bg-[#151515] relative -z-10 {clazz}">
	<Lines />
	<slot />
	{#if renderSquiggly}
		<SquigglyDark
			class="absolute left-0 right-0 w-full bottom-0"
			style="transform: translateY(calc(100% - 1px));"
		/>
	{/if}
</div>
