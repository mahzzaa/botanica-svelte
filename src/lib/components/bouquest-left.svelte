<script>
	import bouquest from '$lib/assets/img/bouquest.png';
</script>

<div
	class="flex flex-col justify-center items-center
   w-full 2xl:h-full xl:h-full lg:h-full md:h-full h-screen space-y-32 my-20 mb-64"
>
	<p class="moniqa text-[#ca7e8d] text-6xl">Unique bouquets for you</p>
	<div
		class="w-full 2xl:h-64 xl:h-64 lg:h-64 md:h-64 h-screen
    2xl:py-0 xl:py-0 lg:py-0 md:py-0 py-20
    grid 2xl:grid-cols-2 xl:grid-cols-2 lg:grid-cols-2 md:grid-cols-2 grid-cols-1
    justify-center items-center relative
    2xl:bg-gradient-to-l xl:bg-gradient-to-l lg:bg-gradient-to-l md:bg-gradient-to-l
    bg-none from-[#d092a0] to-[#dcc5d0]"
	>
		<div
			class="2xl:w-2/3 xl:w-2/3 lg:w-2/3 md:w-2/3 w-full col-start-1
      2xl:ml-44 xl:ml-40 lg:ml-32 md:ml-20 ml-0
      flex flex-col justify-center
      2xl:items-start xl:items-start lg:items-start md:items-start items-center
      2xl:py-0 xl:py-0 lg:py-5 md:py-5 py-10 pt-16
      2xl:text-start xl:text-start lg:text-start md:text-start text-center text-white
      2xl:bg-none xl:bg-none lg:bg-none md:bg-none bg-gradient-to-l from-[#d092a0] to-[#dcc5d0]
      font-gilroy
      2xl:space-y-7 xl:space-y-7 lg:space-y-3 md:space-y-3 space-y-3"
		>
			<h1 class="text-5xl text-white moniqa">Action</h1>
			<p class="2xl:w-full xl:w-full lg:w-full md:w-full w-5/6 text-xl">
				For orders over 10,000 rubles, free delivery within the city!
			</p>
			<button
				class="order flex justify-between border border-white hover:border-[#7a9077] hover:text-[#7a9077]
         px-5 py-2"
			>
				ORDER
				<span class="ml-20">
					<svg class="w-6" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
						<g id="SVGRepo_bgCarrier" stroke-width="0"></g>
						<g id="SVGRepo_tracerCarrier" stroke-linecap="round" stroke-linejoin="round"></g>
						<g id="SVGRepo_iconCarrier">
							<path
								fill-rule="evenodd"
								clip-rule="evenodd"
								d="M17.6492 11.2501L12.7904 6.53852L13.8346 5.46167L20.5774 12.0001L13.8346 18.5385L12.7904 17.4617L17.6492 12.7501H3V11.2501H17.6492Z"
								fill="#ffffff"
							></path>
						</g>
					</svg>
				</span>
			</button>
		</div>

		<div
			class="image flex justify-center items-center absolute
    2xl:-top-2 xl:-top-2 lg:-top-2 md:-top-2 -top-16
    2xl:right-40 xl:right-52 lg:right-32 md:right-40 right-44"
		>
			<!-- box -->
			<div class="w-[200px] h-[300px] left-3 border border-[#7a9077] absolute"></div>
			<!-- img -->
			<div class="z-10 w-[200px]">
				<img class="" src={bouquest} alt="" />
			</div>
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

	.order:hover svg path {
		fill: #7a9077;
	}
</style>
