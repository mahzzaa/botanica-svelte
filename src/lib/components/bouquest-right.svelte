<script>
	import bouquest from '$lib/assets/img/bouquest.png';
</script>

<div
	class="flex flex-col justify-center items-center w-full 2xl:h-full xl:h-full lg:h-full md:h-full h-screen space-y-32 my-20"
>
	<p class="moniqa text-[#ca7e8d] text-6xl">Unique bouquets for you</p>
	<div
		class="w-full 2xl:h-64 xl:h-64 lg:h-64 md:h-64 h-screen
    2xl:py-0 xl:py-0 lg:py-0 md:py-0 py-20
    grid 2xl:grid-cols-2 xl:grid-cols-2 lg:grid-cols-2 md:grid-cols-2 grid-cols-1
    justify-center items-center relative 2xl:bg-gradient-to-l xl:bg-gradient-to-l lg:bg-gradient-to-l md:bg-gradient-to-l bg-none from-[#d092a0] to-[#dcc5d0]"
	>
		<div
			class="image flex justify-center items-center absolute
      2xl:-top-2 xl:-top-2 lg:-top-2 md:-top-2 -top-16
      2xl:left-40 xl:left-52 lg:left-32 md:left-40 left-44"
		>
			<!-- box -->
			<div class="w-[200px] h-[300px] left-3 border border-[#7a9077] absolute"></div>
			<!-- img -->
			<div class="z-10 w-[200px]">
				<img class="" src={bouquest} alt="" />
			</div>
		</div>

		<div
			class="2xl:w-2/3 xl:w-2/3 lg:w-2/3 md:w-2/3 w-full col-start-2
      flex flex-col justify-center items-center 2xl:py-0 xl:py-0 lg:py-5 md:py-5 py-10 pt-16
      2xl:text-wrap xl:text-wrap lg:text-wrap md:text-wrap text-center text-white
      2xl:bg-none xl:bg-none lg:bg-none md:bg-none bg-gradient-to-l from-[#d092a0] to-[#dcc5d0]
      font-gilroy
      2xl:space-y-7 xl:space-y-7 lg:space-y-3 md:space-y-3 space-y-3"
		>
			<p class="2xl:w-full xl:w-full lg:w-full md:w-full w-5/6">
				Botanika is an online store of designer bouquets.
			</p>

			<p class="2xl:w-full xl:w-full lg:w-full md:w-full w-5/6">
				Our range is very flexible and depends on the season. We treat both our clients and their
				color with care, caring for them and transporting them carefully.
			</p>
			<p class="2xl:w-full xl:w-full lg:w-full md:w-full w-5/6">
				Treat yourself and your loved ones with a special bouquet
			</p>
		</div>
	</div>
</div>

<style>
	@import url('https://fonts.cdnfonts.com/css/gilroy-light');

	@font-face {
		font-family: 'Moniqa SemiBold Display';
		src: url('$lib/assets/fonts/Moniqa-SemiBoldDisplay.otf') format('opentype');
		font-weight: 800; /* SemiBold is often considered 600 weight */
		font-style: normal;
	}

	.moniqa {
		font-family: 'Moniqa SemiBold Display', sans-serif;
	}

	.font-gilroy {
		font-family: 'Gilroy-light', sans-serif;
	}
</style>
