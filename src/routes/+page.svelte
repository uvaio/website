<script>
	import Header from '../components/Header.svelte';
	import Table from '../components/Table.svelte';
	import Fab from '../components/Fab.svelte';

	import SectionOne from '../components/SectionOne.svelte';
	import SectionTwo from '../components/SectionTwo.svelte';
	import SectionThree from '../components/SectionThree.svelte';
	import SectionFour from '../components/SectionFour.svelte';
</script>

<svelte:head>
	<title>Above the Surface</title>
	<link rel="icon" type="image/svg" href="/images/logo.svg" />
	<link rel="icon" href="/images/logo.png" type="image/png" />
	<link rel="stylesheet" href="remedy.css" />
	<link rel="stylesheet" href="general.css" />
	<script src="observer.js" defer></script>

	<link rel="preconnect" href="https://fonts.googleapis.com" />
	<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
	<link
		href="https://fonts.googleapis.com/css2?family=IBM+Plex+Mono:wght@300;400;500;700&family=IBM+Plex+Sans:wght@100;300;400;500;700&display=swap"
		rel="stylesheet"
	/>
</svelte:head>

<Header />
<Table />

<main>
	<SectionOne />
	<SectionTwo />
	<SectionThree />
	<SectionFour />
</main>

<Fab />
