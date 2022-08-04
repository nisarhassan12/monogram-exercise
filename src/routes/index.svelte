<script>
	import Api from '$lib/components/api.svelte';
	import AuditScores from '$lib/components/audit-scores.svelte';
	import FallingLogos from '$lib/components/falling-logos.svelte';
	import Footer from '$lib/components/footer.svelte';
	import Javascript from '$lib/components/javascript.svelte';
	import LinesGrid from '$lib/components/layout/lines-grid.svelte';
	import Markup from '$lib/components/markup.svelte';
	import Hero from '../lib/components/hero.svelte';
</script>

<Hero />

<main class="w-full">
	<Javascript />
	<LinesGrid class="-mt-56 sm:-mt-96 xl:-mt-[560px] pb-[800px]" renderSquiggly={true}>
		<FallingLogos />
	</LinesGrid>
	<Api />
	<Markup />
	<LinesGrid>
		<AuditScores />
		<Footer />
	</LinesGrid>
</main>
