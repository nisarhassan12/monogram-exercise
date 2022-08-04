<script lang="ts">
	let clazz = '';
	export { clazz as class };
	export let type: 'h1' | 'h2' = 'h2';
	export let size: 'h1' | 'h3' = 'h1'

	const sizeToClassesMap = {
		h1: "text-5xl sm:text-6xl md:text-8xl 2xl:text-9xl",
		h3: "text-4xl md:text-6xl 2xl:text-7xl"
	}
</script>

<svelte:element 
	this={type} 
	class="font-[900] tracking-[-0.039em] leading-normal sm:leading-relaxed md:leading-[152px] {sizeToClassesMap[size]} {clazz}"
>
	<slot />
</svelte:element>
