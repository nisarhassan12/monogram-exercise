<script>
	import Heading from './heading.svelte';
	import Container from './layout/container.svelte';
	import Paragraph from './paragraph.svelte';
	import Scores from './scores.svelte';
</script>

<Container>
	<div
		class="max-w-[1204px] mx-auto pt-32 pb-20 xl:pb-56 px-8 xl:px-16 backdrop-blur-[120px] rounded-[68px] mix-blend-normal text-center transform -translate-y-28"
		style="background: linear-gradient(25.39deg, rgba(255, 255, 255, 0.024) 18.54%, rgba(123, 245, 93, 0.108) 62.25%); border: 1px solid;border-image-source: radial-gradient(65.6% 145.73% at 90.52% 2.09%, rgba(255, 255, 255, 0.3) 2.08%, rgba(255, 255, 255, 0) 53.65%, rgba(123, 245, 93, 0.135) 100%) /* warning: gradient uses a rotation that is not supported by CSS and may not behave as expected */;
		"
	>
		<Heading class="text-white mb-12 xl:mb-24" size="h3">top audit scores</Heading>

		<Scores />

		<div class="space-y-6 sm:space-y-9 max-w-3xl mx-auto mt-16 xl:mt-32">
			<Paragraph size="lg" class="text-[#C7C7C7] mix-blend-color-dodge">
				Search engines, business stakeholders, and end-users gauge a website’s value using metric
				tools like Google Lighthouse, which measures site performance, SEO, and accessibility.
			</Paragraph>

			<Paragraph size="lg" class="text-[#C7C7C7] mix-blend-color-dodge">
				Performance is one of the most difficult scores to get to 100. This is especially true in a
				time when users demand JavaScript-heavy, highly-interactive web experiences.
			</Paragraph>

			<Paragraph size="lg" class="text-[#C7C7C7] mix-blend-color-dodge">
				A Jamstack website, delivering SEO-friendly, lean & clean HTML in milliseconds, promises
				higher search-engine ranking and a more positive, responsive end-user experience.
			</Paragraph>
		</div>
	</div>
</Container>
