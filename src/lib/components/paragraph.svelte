<script lang="ts">
	let clazz = '';
	export { clazz as class };
	export let size: 'lg' | 'md' | 'sm' = 'sm';

	const sizeToClassesMap = {
		lg: 'text-lg sm:text-[1.375rem] xl:text-[1.625rem] leading-10 font-light',
		md: 'text-lg sm:text-xl xl:text-2xl leading-10 font-light',
		sm: 'md:text-lg md:leading-9 font-light'
	}
</script>

<p class="{sizeToClassesMap[size]} {clazz}">
	<slot />
</p>