<script>
	import { onMount } from 'svelte';
	import { bind } from '../../src/lib/nice-select2.js';

	onMount((async) => {
		bind(document.querySelector('.function'));
		bind(document.querySelector('.country'));
		bind(document.querySelector('.time'));
		bind(document.querySelector('.material'));
	});
</script>

<div class="filter">
	<div class="sentence">
		<h3>Show me objects of</h3>
		<select class="function">
			<option selected="selected" value="functional">functional property</option>
			<option value="communication">Communication & Exchange</option>
			<option value="building">Building & Structures</option>
			<option value="personal">Personal Artefacts and Clothing</option>
			<option value="science">Science & Technology</option>
		</select>
		<h3>that were used by</h3>
		<h3>from country</h3>
		<select class="country">
			<option selected="selected" value="country">country of origin</option>
			<option value="nl">Netherlands</option>
			<option value="eng">England</option>
			<option value="fr">France</option>
			<option value="de">Germany</option>
		</select>
		<h3>in time period</h3>
		<select class="time">
			<option selected="selected" value="time">time period</option>
			<option value="1200-1400">1200-1400</option>
			<option value="1400-1600">1400-1600</option>
			<option value="1600-1700">1600-1700</option>
			<option value="1700-1800">1700-1800</option>
			<option value="1800-2000">1800-2000</option>
		</select>
		<h3>that are made from</h3>
		<select class="material">
			<option selected="selected" value="materials">material</option>
			<option value="plastic">Plastic</option>
			<option value="steel">Steel</option>
			<option value="wood">Wood</option>
			<option value="cotton">Cotton</option>
		</select>
	</div>
</div>

<style>
	.filter {
		background: var(--secondary-color);
		color: var(--primary-color);
		height: 20vh;
		padding: 2em 10vw;
	}

	.nice-select {
		margin: 2em !important;
		border-radius: 0px !important;
		color: black !important;
	}

	.nice-select .nice-select-dropdown {
		color: black !important;
	}

	h3 {
		font-size: 2em;
	}

	.sentence {
		display: flex;
		flex-wrap: wrap;
		align-items: center;
	}
</style>
