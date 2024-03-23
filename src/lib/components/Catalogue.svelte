<script>
	import flower from '../assets/img/flower2.jpeg';
</script>

<div class="flex flex-col justify-center items-center my-28 space-y-8 font-gilroy">
	<h1 class="moniqa text-[#ca7e8d] text-7xl">Catalogue</h1>

	<div class="category flex text-[#7a9077] space-x-6 font-light pt-10">
		<button
			class=" px-3 py-2 border-transparent focus:border focus:border-[#7a9077] hover:border hover:border-[#7a9077]"
		>
			Maxi bouquests
		</button>
		<button
			class=" px-3.5 py-2.5 border border-transparent focus:border focus:border-[#7a9077] hover:border hover:border-[#7a9077]"
		>
			Mini bouquests
		</button>
		<button
			class=" px-3.5 py-2.5 border border-[#7a9077] focus:border focus:border-[#7a9077] hover:border hover:border-[#7a9077]"
		>
			Wedding bouquests
		</button>
		<button
			class=" px-3.5 py-2.5 border border-transparent focus:border focus:border-[#7a9077] hover:border hover:border-[#7a9077]"
		>
			Author's bouquests
		</button>
		<button
			class=" px-3.5 py-2.5 border border-transparent focus:border focus:border-[#7a9077] hover:border hover:border-[#7a9077]"
		>
			Dried flowers
		</button>
	</div>

	<div class="grid grid-cols-3 gap-x-10 pt-16">
		<div class="flex justify-center items-center relative">
			<img class="w-[200px]" src={flower} alt="" />
			<p class="absolute bottom-12 left-10 text-white">300$</p>
		</div>
		<div class="flex justify-center items-center relative">
			<div class="border border-[#7a9077] w-[250px] h-[370px] absolute left-5 bottom-5"></div>
			<img class="w-[250px] z-10" src={flower} alt="" />
			<p class="absolute bottom-5 left-5 text-white z-10">300$</p>
			<button
				class="absolute bottom-5 right-5 text-white z-10 text-sm border border-white px-3 py-2
        hover:bg-white hover:bg-opacity-40 transition delay-100">ADD TO CART</button
			>
		</div>
		<div class="flex justify-center items-center relative">
			<img class="w-[200px]" src={flower} alt="" />
			<p class="absolute bottom-12 left-10 text-white">300$</p>
		</div>
	</div>
	<div class="flex items-center justify-between w-full space-x-7">
		<!-- left flesh -->
		<svg
			fill="#000000"
			viewBox="0 0 24 24"
			id="left-arrow"
			xmlns="http://www.w3.org/2000/svg"
			class="icon line w-8 hover:scale-105 cursor-pointer"
			><g id="SVGRepo_bgCarrier" stroke-width="0"></g><g
				id="SVGRepo_tracerCarrier"
				stroke-linecap="round"
				stroke-linejoin="round"
			></g><g id="SVGRepo_iconCarrier"
				><path
					id="primary"
					d="M21,12H3M6,9,3,12l3,3"
					style="fill: none; stroke: #7a9077; stroke-linecap: round; stroke-linejoin: round; stroke-width: 1.5;"
				></path></g
			></svg
		>

		<!-- dots -->

		<div class="flex justify-center items-center dote space-x-3">
			<div
				class="w-1.5 h-1.5 bg-[#7a9077] opacity-40 rounded-full hover:cursor-pointer hover:w-2 hover:h-2"
			></div>
			<div
				class="w-1.5 h-1.5 bg-[#7a9077] opacity-40 active rounded-full hover:cursor-pointer hover:w-2 hover:h-2"
			></div>
			<div
				class="w-1.5 h-1.5 bg-[#7a9077] opacity-40 rounded-full hover:cursor-pointer hover:w-2 hover:h-2"
			></div>
		</div>

		<!-- right flesh -->
		<svg
			fill="#000000"
			viewBox="0 0 24 24"
			id="right-arrow"
			xmlns="http://www.w3.org/2000/svg"
			class="icon line w-8 hover:scale-105 cursor-pointer"
			><g id="SVGRepo_bgCarrier" stroke-width="0"></g><g
				id="SVGRepo_tracerCarrier"
				stroke-linecap="round"
				stroke-linejoin="round"
			></g><g id="SVGRepo_iconCarrier"
				><path
					id="primary"
					d="M3,12H21m-3,3,3-3L18,9"
					style="fill: none; stroke: #7a9077; stroke-linecap: round; stroke-linejoin: round; stroke-width: 1.5;"
				></path></g
			></svg
		>
	</div>
</div>

<style>
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

	.active {
		padding: px-3 py-2;
		border: 1px solid #7a9077;
		transition: border-color 0.3s;
	}

	.dote .active {
		opacity: 1;
	}
</style>
