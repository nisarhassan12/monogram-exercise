<script>
	import Heading from './heading.svelte';
	import Container from './layout/container.svelte';
	import Paragraph from './paragraph.svelte';
</script>

<section class="px-1 xs:px-6 md:px-12">
	<div
		class="relative bg-[url('/images/orange-square.png')] bg-contain bg-no-repeat max-w-[1400px] text-center mx-auto pt-2 sm:pt-4 md:mt-0 md:pt-12 xl:pt-24 z-10"
	>
		<Container>
			<Heading class="text-white">javascript</Heading>
			<Paragraph class="max-w-xl mx-auto text-white md:mt-5 2xl:mt-11">
				Statically generated pages are brought to life with client-side JavaScript libraries and
				frameworks, such as Algolia and Next.js.
			</Paragraph>
			<img src="/images/retro-computer.png" alt="Retro Computer" class="mx-auto mt-3 xs:mt-10 2xl:mt-20 max-w-[50vw] 2xl:max-w-none" />
		</Container>
		<!-- Since this graphic is just for presentational purposes I haved added aria-hidden to make it so that it does not appear in the Accessibility tree. -->
		<img
			src="/svgs/squiggly-arrow.svg"
			alt=""
			aria-hidden="true"
			class="absolute hidden lg:block top-44 xl:top-64 right-10 2xl:right-24 max-h-[25vw] 2xl:max-h-auto"
		/>
	</div>
</section>
