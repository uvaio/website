<script>
	import HeaderSmall from '../../components/HeaderSmall.svelte';
	import Back from '../../components/Back.svelte';
	import Filter from '../../components/Filter.svelte';
	import Grid from '../../components/Grid.svelte';
</script>

<svelte:head>
	<title>Above the Surface</title>
	<link rel="icon" type="image/svg" href="/images/logo.svg" />
	<link rel="icon" href="/images/logo.png" type="image/png" />
	<link rel="stylesheet" href="remedy.css" />
	<link rel="stylesheet" href="general.css" />
	<link rel="stylesheet" href="nice-select2.css" />

	<link rel="preconnect" href="https://fonts.googleapis.com" />
	<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
	<link
		href="https://fonts.googleapis.com/css2?family=IBM+Plex+Mono:wght@300;400;500;700&family=IBM+Plex+Sans:wght@100;300;400;500;700&display=swap"
		rel="stylesheet"
	/>
</svelte:head>

<HeaderSmall />
<Back />
<Filter />
<Grid />
