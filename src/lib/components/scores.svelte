<ul class="flex flex-wrap justify-center gap-12 xl:gap-16 list-none">
	{#each Array(4) as _, i}
		<li
			class="relative flex justify-center items-center rounded-full h-32 w-32 sm:h-40 sm:w-40 xl:h-52 xl:w-52 border-4 border-solid border-[#EFFFE2] font-bold text-4xl sm:text-5xl xl:text-6xl leading-[76px] text-[#EFFFE2]"
			style="text-shadow:0px 0px 12px #53FB2A, 0px 0px 42px #E9E11F, 0px 0px 61px #53FB2A;
			box-shadow:
				inset 0px 0px 12px #53FB2A, 0 0 12px #53FB2A;
			"
		>
			100
			<span class="absolute right-0 transform translate-x-1 h-6 xl:h-8 w-[5px] rounded-full bg-[#21291f]" style="box-shadow: 0 0 20px 10px #121212"></span>
		</li>
	{/each}
</ul>
