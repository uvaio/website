<script>
	import Stats from '../components/Stats.svelte';
</script>

<section>
	<h1 id="introduction">Introduction</h1>
	<p>
		From 2003 to 2012 excavations took place for the creation of the <strong
			>North/South metro line in Amsterdam</strong
		>. At Damrak and Rokin, which are unlikely archaeological sites due to being in the city center,
		archaeologists had a chance to physically access the riverbed.
	</p>
	<p>
		During these excavations in the Amstel over <strong>700,000 objects</strong> were preserved which
		resulted in a large archaeological collection. This website acts as an overview of the Below the
		Surface dataset.
	</p>
	<Stats />
</section>

<style>
	h1,
	p,
	.button {
		opacity: 0;
		animation: left 300ms ease 1s forwards;
	}

	@keyframes left {
		0% {
			transform: translateY(1em);
			opacity: 0;
		}

		100% {
			transform: translateY(0em);
			opacity: 1;
		}
	}

	section {
		height: 65vh;
	}
</style>
