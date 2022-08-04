<script lang="ts">
	import FallingLogo from './falling-logo.svelte';
	import Container from './layout/container.svelte';

	const react = {
		src: '/svgs/reactjs.svg',
		alt: 'React JS'
	};

	const svelte = {
		src: '/svgs/sveltejs.svg',
		alt: 'Svelte JS'
	};

	const next = {
		src: '/svgs/nextjs.svg',
		alt: 'Next JS'
	};

	const vue = {
		src: '/svgs/vuejs.svg',
		alt: 'Vue JS'
	};
</script>

<Container class="pt-[300px] text-center">
	<div class="grid grid-cols-4">
		<div class="flex flex-col">
			<FallingLogo image={react} class="my-96" styles="filter: drop-shadow(2px -5px 5px #fff);" parentStyles="filter: drop-shadow(0 -40px 20px #fff);" />
			<FallingLogo image={svelte} class="opacity-30" styles="filter: drop-shadow(1px 1px 1px #ddd);" parentStyles="filter: drop-shadow(0 -20px 10px #888);"/>
		</div>
		<div class="flex flex-col">
			<FallingLogo image={next} class="mt-[600px] mb-[500px]" styles="filter: drop-shadow(2px -5px 10px #fff);" parentStyles="filter: drop-shadow(0 -40px 10px #555);"/>
			<FallingLogo image={react} class="opacity-20" styles="filter: drop-shadow(-1px -1px 2px #bbb);"/>
		</div>
		<div class="flex flex-col">
			<FallingLogo image={vue} class="mt-[800px] opacity-50" styles="filter: drop-shadow(2px -2px 5px #aaa);" parentStyles="filter: drop-shadow(0 -20px 20px #ccc);"/>
		</div>
		<div class="flex flex-col">
			<FallingLogo image={next} class="mt-24" styles="filter: drop-shadow(2px -5px 10px #fff);" parentStyles="filter: drop-shadow(0 -40px 10px #555);" />
			<FallingLogo image={react} class="mt-96 mb-[600px]" styles="filter: drop-shadow(2px -5px 5px #fff);" parentStyles="filter: drop-shadow(0 -40px 20px #fff);"/>
			<FallingLogo image={svelte} class="opacity-20 transform translate-y-20" styles="filter: drop-shadow(-1px -1px 2px #bbb);"/>
		</div>
	</div>
</Container>
