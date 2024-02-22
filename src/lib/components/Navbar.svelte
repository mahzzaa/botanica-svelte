<script>
	let clicked = false;

	const handleClick = () => {
		clicked = !clicked;
	};

	const resetClick = () => {
		clicked = false;
	};

	const links = [
		{
			url: '/',
			linkText: 'Home'
		},
		{
			url: '/about',
			linkText: 'About'
		},
		{
			url: '/catalog',
			linkText: 'Catalog'
		},
		{
			url: '/review',
			linkText: 'Review'
		},
		{
			url: '/stock',
			linkText: 'Stock'
		},
		{
			url: '/contacts',
			linkText: 'Contacts'
		}
	];
</script>

<nav class="relative grid grid-cols-6 justify-center items-center font-gilroy py-2 px-3">
	<div class=" col-span-1 justify-start flex">
		<a href="/" class="font-callina text-4xl font-bold text-[#7a9077] hover:cursor-pointer">
			Botanica
		</a>
	</div>

	<div
		class="2xl:col-span-3 xl:col-span-3 lg:col-span-3 md:col-span-3 col-span-5
     flex space-x-4
     2xl:justify-center xl:justify-center lg:justify-center md:justify-end justify-end items-center"
	>
		{#each links as link}
			<div
				class="2xl:block xl:block lg:block md:block hidden"
				on:click={resetClick}
				on:keypress={resetClick}
				role="button"
				tabindex="0"
			>
				<a
					href={link.url}
					class="hover:border-b hover:border-b-[#7a9077] text-[#7a9077] font-bold space-x-4 pb-3"
				>
					{link.linkText}
				</a>
			</div>
		{/each}
		<!-- icon wrapper -->
		<div
			class="2xl:hidden xl:hidden lg:hidden md:hidden block"
			on:click={handleClick}
			on:keypress={handleClick}
			role="button"
			tabindex="0"
		>
			<i
				class={`${clicked ? 'fa fa-times' : 'fas fa-bars'} text-2xl text-[#7a9077] hover:text-[#ca7e8d] `}
			/>
		</div>
	</div>

	<!-- contact us  -->
	<div
		class=" text-[#7a9077] col-span-2
2xl:block xl:block lg:block md:block hidden"
	>
		<div class="flex justify-end items-center space-x-3">
			<!-- phone svg icon -->
			<svg
				class="w-8 hover:fill-[#ca7e8d]"
				fill="#7a9077"
				viewBox="0 0 32 32"
				version="1.1"
				xmlns="http://www.w3.org/2000/svg"
			>
				<g id="SVGRepo_bgCarrier" stroke-width="0"></g>
				<g id="SVGRepo_tracerCarrier" stroke-linecap="round" stroke-linejoin="round"></g>
				<g id="SVGRepo_iconCarrier">
					<title>phone</title>
					<path
						d="M0 10.375c0 0.938 0.344 1.969 0.781 3.063s1 2.125 1.438 2.906c1.188 2.063 2.719 4.094 4.469 5.781s3.813 3.094 6.125 3.938c1.344 0.531 2.688 1.125 4.188 1.125 0.75 0 1.813-0.281 2.781-0.688 0.938-0.406 1.781-1.031 2.094-1.781 0.125-0.281 0.281-0.656 0.375-1.094 0.094-0.406 0.156-0.813 0.156-1.094 0-0.156 0-0.313-0.031-0.344-0.094-0.188-0.313-0.344-0.563-0.5-0.563-0.281-0.656-0.375-1.5-0.875-0.875-0.5-1.781-1.063-2.563-1.469-0.375-0.219-0.625-0.313-0.719-0.313-0.5 0-1.125 0.688-1.656 1.438-0.563 0.75-1.188 1.438-1.625 1.438-0.219 0-0.438-0.094-0.688-0.25s-0.5-0.281-0.656-0.375c-2.75-1.563-4.594-3.406-6.156-6.125-0.188-0.313-0.625-0.969-0.625-1.313 0-0.406 0.563-0.875 1.125-1.375 0.531-0.469 1.094-1.031 1.094-1.719 0-0.094-0.063-0.375-0.188-0.781-0.281-0.813-0.656-1.75-0.969-2.656-0.156-0.438-0.281-0.75-0.313-0.906-0.063-0.094-0.094-0.219-0.125-0.375s-0.094-0.281-0.125-0.406c-0.094-0.281-0.25-0.5-0.406-0.625-0.156-0.063-0.531-0.156-0.906-0.188-0.375 0-0.813-0.031-1-0.031-0.094 0-0.219 0-0.344 0.031h-0.406c-1 0.438-1.719 1.313-2.25 2.344-0.5 1.031-0.813 2.188-0.813 3.219z"
					>
					</path>
				</g>
			</svg>
			<!-- phone number -->
			<p>8-800-555-00-00</p>

			<!-- add to basket svg icon -->
			<svg
				class="w-8 hover:fill-[#ca7e8d]"
				fill="#7A9077"
				viewBox="0 0 32 32"
				version="1.1"
				xmlns="http://www.w3.org/2000/svg"
				stroke="#7A9077"
				stroke-width="0.00032"
			>
				<g id="SVGRepo_bgCarrier" stroke-width="0"></g>
				<g id="SVGRepo_tracerCarrier" stroke-linecap="round" stroke-linejoin="round"></g>
				<g id="SVGRepo_iconCarrier">
					<path
						d="M27 4.96h-5.975v-1.918c0-1.655-1.346-3-3-3h-3.989c-1.655 0-3 1.345-3 3v1.918h-6.037c-1.104 0-2 0.896-2 2v22.999c0 1.105 0.896 2 2 2h22c1.105 0 2-0.895 2-2v-22.999c0-1.104-0.895-2-2-2h0zM13.037 3.042c0-0.552 0.448-1 1-1h3.989c0.552 0 1 0.448 1 1v1.918h-5.989v-1.918zM27 29.959h-22v-22.999h6.037v2.058s-0.027 0.999 0.994 0.999c1.125 0 1.006-0.999 1.006-0.999v-2.058h5.989v2.058s-0.067 1.004 0.996 1.004c1 0 1.004-1.004 1.004-1.004v-2.058h5.974v22.999z"
					>
					</path>
				</g>
			</svg>
		</div>
	</div>
	<!-- side navbar -->
	{#if clicked}
		<div class="absolute z-10 top-0 h-screen w-full bg-white flex flex-col py-2 px-3 space-y-5">
			<!-- side navbar icon wrapper -->
			<div
				class="w-full flex justify-end"
				on:click={handleClick}
				on:keypress={handleClick}
				role="button"
				tabindex="0"
			>
				<i
					class={`${clicked ? 'fa fa-times' : 'fas fa-bars'} text-2xl text-[#7a9077] hover:text-[#ca7e8d] `}
				/>
			</div>

			<!-- side navbar links -->
			{#each links as link}
				<div
					class="pb-3 border-b border-b-transparent hover:border-b hover:border-b-[#7a9077]"
					on:click={resetClick}
					on:keypress={resetClick}
					role="button"
					tabindex="0"
				>
					<a href={link.url} class="text-[#7a9077] font-bold space-x-4 text-xl h-full">
						{link.linkText}
					</a>
				</div>
			{/each}

			<!-- contact us  -->
			<div class=" bottom-0 text-[#7a9077] w-full">
				<div class="flex justify-center items-end space-x-3">
					<!-- phone svg icon -->
					<svg
						class="w-8 hover:fill-[#ca7e8d]"
						fill="#7a9077"
						viewBox="0 0 32 32"
						version="1.1"
						xmlns="http://www.w3.org/2000/svg"
					>
						<g id="SVGRepo_bgCarrier" stroke-width="0"></g>
						<g id="SVGRepo_tracerCarrier" stroke-linecap="round" stroke-linejoin="round"></g>
						<g id="SVGRepo_iconCarrier">
							<title>phone</title>
							<path
								d="M0 10.375c0 0.938 0.344 1.969 0.781 3.063s1 2.125 1.438 2.906c1.188 2.063 2.719 4.094 4.469 5.781s3.813 3.094 6.125 3.938c1.344 0.531 2.688 1.125 4.188 1.125 0.75 0 1.813-0.281 2.781-0.688 0.938-0.406 1.781-1.031 2.094-1.781 0.125-0.281 0.281-0.656 0.375-1.094 0.094-0.406 0.156-0.813 0.156-1.094 0-0.156 0-0.313-0.031-0.344-0.094-0.188-0.313-0.344-0.563-0.5-0.563-0.281-0.656-0.375-1.5-0.875-0.875-0.5-1.781-1.063-2.563-1.469-0.375-0.219-0.625-0.313-0.719-0.313-0.5 0-1.125 0.688-1.656 1.438-0.563 0.75-1.188 1.438-1.625 1.438-0.219 0-0.438-0.094-0.688-0.25s-0.5-0.281-0.656-0.375c-2.75-1.563-4.594-3.406-6.156-6.125-0.188-0.313-0.625-0.969-0.625-1.313 0-0.406 0.563-0.875 1.125-1.375 0.531-0.469 1.094-1.031 1.094-1.719 0-0.094-0.063-0.375-0.188-0.781-0.281-0.813-0.656-1.75-0.969-2.656-0.156-0.438-0.281-0.75-0.313-0.906-0.063-0.094-0.094-0.219-0.125-0.375s-0.094-0.281-0.125-0.406c-0.094-0.281-0.25-0.5-0.406-0.625-0.156-0.063-0.531-0.156-0.906-0.188-0.375 0-0.813-0.031-1-0.031-0.094 0-0.219 0-0.344 0.031h-0.406c-1 0.438-1.719 1.313-2.25 2.344-0.5 1.031-0.813 2.188-0.813 3.219z"
							>
							</path>
						</g>
					</svg>
					<!-- phone number -->
					<p>8-800-555-00-00</p>

					<!-- add to basket svg icon -->
					<svg
						class="w-8 hover:fill-[#ca7e8d]"
						fill="#7A9077"
						viewBox="0 0 32 32"
						version="1.1"
						xmlns="http://www.w3.org/2000/svg"
						stroke="#7A9077"
						stroke-width="0.00032"
					>
						<g id="SVGRepo_bgCarrier" stroke-width="0"></g>
						<g id="SVGRepo_tracerCarrier" stroke-linecap="round" stroke-linejoin="round"></g>
						<g id="SVGRepo_iconCarrier">
							<path
								d="M27 4.96h-5.975v-1.918c0-1.655-1.346-3-3-3h-3.989c-1.655 0-3 1.345-3 3v1.918h-6.037c-1.104 0-2 0.896-2 2v22.999c0 1.105 0.896 2 2 2h22c1.105 0 2-0.895 2-2v-22.999c0-1.104-0.895-2-2-2h0zM13.037 3.042c0-0.552 0.448-1 1-1h3.989c0.552 0 1 0.448 1 1v1.918h-5.989v-1.918zM27 29.959h-22v-22.999h6.037v2.058s-0.027 0.999 0.994 0.999c1.125 0 1.006-0.999 1.006-0.999v-2.058h5.989v2.058s-0.067 1.004 0.996 1.004c1 0 1.004-1.004 1.004-1.004v-2.058h5.974v22.999z"
							>
							</path>
						</g>
					</svg>
				</div>
			</div>
		</div>
	{/if}
</nav>

<style>
	/* logo */
	@import url('https://fonts.cdnfonts.com/css/callina');

	/* navbar */
	@import url('https://fonts.cdnfonts.com/css/gilroy-bold');

	.font-callina {
		font-family: 'Callina', sans-serif;
	}

	.font-gilroy {
		font-family: 'Gilroy-Light', sans-serif;
	}
</style>
