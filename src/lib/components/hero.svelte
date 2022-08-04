<script>
	import Heading from './heading.svelte';

	import Container from './layout/container.svelte';
	import Paragraph from './paragraph.svelte';
</script>

<Container class="mt-16 md:mt-32 2xl:mt-40 relative">
	<header>
		<Heading type="h1" class="flex gap-2 sm:block">
			jamstack <span
				class="2xl:ml-5 bg-gradient-to-r from-[#fec087] to-[#cc77a1] bg-clip-text text-transparent"
				>101</span
			>
		</Heading>

		<div class="flex items-start">
			<div class="w-96 md:w-auto">
				<Paragraph
					class="mr-4 md:mx-6 xl:mx-8 2xl:mx-12 md:mt-5 xl:mt-11 text-[#757575] w-72 md:w-[420px] xl:w-[520px]"
				>
					Lorem ipsum dolor sit amet, consectetur adipiscing elit. Arcu augue massa, tincidunt proin
					nunc viverra tristique tempor, ipsum.&nbsp;At lectus vel pretium tempor ut dui vivamus
					sit.
				</Paragraph>
				<img
					src="/svgs/mouse-line.svg"
					alt="Scroll Indicator"
					class="mx-auto mb-10 h-[40vw] lg:h-96 2xl:h-auto mt-10 lg:mt-24"
				/>
			</div>
			<!-- Since this graphic is just for presentational purposes I haved added aria-hidden to make it so that it does not appear in the Accessibility tree. -->
			<img
				src="/images/hero-graphic.png"
				class="max-w-[30vw] sm:max-w-[50vw] lg:max-w-xl 2xl:max-w-3xl transform sm:translate-x-3 lg:translate-x-16 xl:translate-x-0 sm:-translate-y-20 lg:-translate-y-32 xl:-translate-y-40"
				alt=""
				aria-label="hidden"
			/>
		</div>
	</header>
</Container>
