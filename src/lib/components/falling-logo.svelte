<script lang="ts">
	let clazz = '';
	export { clazz as class };
	export let image: {src: string; alt: string};
	export let styles: string = '';
	export let parentStyles: string = '';
	const { src, alt } = image;
</script>

<div class="flex justify-center" style={parentStyles}>
	<img {src} {alt} class="h-5 w-16 xs:w-auto
	sm:h-8 lg:h-10 {clazz}" style={styles}>
</div>