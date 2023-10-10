<script>
	import { onMount } from 'svelte';
	import { bind } from '../../src/lib/nice-select2.js';

	onMount((async) => {
		bind(document.querySelector('.function'));
		bind(document.querySelector('.culture'));
		bind(document.querySelector('.country'));
		bind(document.querySelector('.time'));
		bind(document.querySelector('.material'));
	});
</script>

<div class="filter">
	<div class="sentence">
		<h3>Give me items of</h3>
		<select class="function">
			<option selected="selected" value="2022">function</option>
			<option value="2021">2021</option>
			<option value="2020">2020</option>
			<option value="2019">2019</option>
			<option value="2018">2018</option>
		</select>
		<h3>that were used by</h3>
		<select class="culture">
			<option selected="selected" value="2022">cultural tribe</option>
			<option value="2021">2021</option>
			<option value="2020">2020</option>
			<option value="2019">2019</option>
			<option value="2018">2018</option>
		</select>
		<h3>from country</h3>
		<select class="country">
			<option selected="selected" value="2022">country of origin</option>
			<option value="2021">2021</option>
			<option value="2020">2020</option>
			<option value="2019">2019</option>
			<option value="2018">2018</option>
		</select>
		<h3>in time period</h3>
		<select class="time">
			<option selected="selected" value="2022">time period</option>
			<option value="2021">2021</option>
			<option value="2020">2020</option>
			<option value="2019">2019</option>
			<option value="2018">2018</option>
		</select>
		<h3>that are made from</h3>
		<select class="material">
			<option selected="selected" value="2022">material</option>
			<option value="2021">2021</option>
			<option value="2020">2020</option>
			<option value="2019">2019</option>
			<option value="2018">2018</option>
		</select>
	</div>
</div>

<style>
	.filter {
		background: #f3f1ed;
		height: 20vh;
		padding: 2em 10vw;
	}

	.nice-select {
		margin: 2em !important;
		border-radius: 0px !important;
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
