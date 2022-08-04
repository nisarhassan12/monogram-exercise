<script lang="ts">
	import Container from './layout/container.svelte';
	import Paragraph from './paragraph.svelte';

	const logos: {
		src: string;
		alt: string;
	}[] = [
		{
			src: '/svgs/sveltejs.svg',
			alt: 'Svelte JS'
		},
		{
			src: '/svgs/nextjs.svg',
			alt: 'Next JS',
		},
		{
			src: '/svgs/reactjs.svg',
			alt: 'React JS'
		},
		{
			src: '/svgs/vuejs.svg',
			alt: 'Vue JS'
		}
	]; 
</script>

<Container class="pt-[600px] pb-[600px] text-center">
	<Paragraph class="text-white">Falling logos are gonna go here.</Paragraph>
	{#each logos as {src, alt} }
		<img {src} {alt} class="h-12">
	{/each}
</Container>
