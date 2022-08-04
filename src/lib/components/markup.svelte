<script>
	import Heading from './heading.svelte';
	import Container from './layout/container.svelte';
	import Paragraph from './paragraph.svelte';
</script>

<section class="mt-32 xl:mt-64 text-center sm:text-left">
	<Container class="flex justify-between">
		<div class="max-w-md sm:min-w-[500px] mx-auto">
			<Heading>markup</Heading>
			<Paragraph size="md" class="mt-5 xl:mt-16">
				When ready for deployment, a static-site generator such as Astro or Next.js is used to
				compile the website. The end result is a collection of pre-rendered HTML pages that can be
				delivered lightning-fast over a CDN like Vercel’s Edge Network.
			</Paragraph>
			<img src="/images/toppled-blocks.png" class="mt-16 w-52 sm:w-[50vw] mx-auto mb-10 sm:mb-0 sm:mx-0" alt="" aria-hidden="true">
		</div>
		<!-- Since this graphic is just for presentational purposes I haved added aria-hidden to make it so that it does not appear in the Accessibility tree. -->
		<img src="/images/block-graphic.png" class="hidden sm:block sm:max-w-[30vw] transfrom -translate-x-20 md:transform-none md:max-w-[50vw] ml-24 2xl:ml-44" alt="" aria-label="hidden" />
	</Container>
	<img src="/images/wall-of-blocks.png" alt="" aria-hidden="true" class="w-full mt-8">
</section>
