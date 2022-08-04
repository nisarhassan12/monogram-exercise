<script>
	import Heading from './heading.svelte';
	import Container from './layout/container.svelte';
	import Paragraph from './paragraph.svelte';
</script>

<Container class="text-center -mt-[450px] md:-mt-[550px] lg:-mt-[700px] z-20">
	<Heading class="text-white mb-5 xl:mb-14">api</Heading>
	<Paragraph class="max-w-3xl mx-auto text-white mb-10 xl:mb-32" size="md">
		At build time, a Jamstack website uses data from one or more APIs to generate markup. These APIs
		can be a headless CMS like Prismic, a database like Supabase, or even a local JSON file!
	</Paragraph>
	<div class="relative rounded-full max-w-4xl mx-auto">
		<img
			src="/images/circle.png"
			alt="Jamstack APIs"
			class="w-full rounded-full shadow-[-15px_-15px_35px_#fff] xl:shadow-[-30px_-30px_80px_#fff]"
		/>
	</div>
</Container>

<style lang="postcss">
	div::before {
		content: '';
		@apply absolute -top-7 -left-7 xl:-top-14 xl:-left-14 h-full w-full -z-10 rounded-full;
		background: linear-gradient(50.94deg, #01A6DC 14.62%, #8801E4 54.03%, #F5CBE1 85.34%);
		filter: blur(40px);
	}
</style>
