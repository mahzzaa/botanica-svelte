<script>
	import Catalogue from '../lib/components/Catalogue.svelte';
	import HeaderLanding from '../lib/components/Header-landing.svelte';
	import BouquestLeft from '../lib/components/bouquest-left.svelte';
	import Bouquest from '../lib/components/bouquest.svelte';
</script>

<!-- YOU CAN DELETE EVERYTHING IN THIS PAGE -->

<div class=" h-full w-full mx-auto flex flex-col justify-center items-center bg-white">
	<HeaderLanding />
	<Bouquest />
	<Catalogue />
	<BouquestLeft />
</div>
