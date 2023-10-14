<script>
	import { onMount } from 'svelte';

	onMount(async () => {
		const buttonForm = document.querySelector('.filterButton');
		const form = document.querySelector('.form');

		buttonForm.addEventListener('click', filter);

		function filter() {
			form.classList.toggle('open');
		}
	});
</script>

<div class="subfilter">
	<div class="search">
		<input type="search" id="site-search" name="q" placeholder="NZD1.00303KST002" />

		<button class="formButton"
			>Search by object tag<svg
				width="24"
				height="24"
				viewBox="0 0 24 24"
				fill="none"
				xmlns="http://www.w3.org/2000/svg"
			>
				<path
					fill-rule="evenodd"
					clip-rule="evenodd"
					d="M18.319 14.4326C20.7628 11.2941 20.542 6.75347 17.6569 3.86829C14.5327 0.744098 9.46734 0.744098 6.34315 3.86829C3.21895 6.99249 3.21895 12.0578 6.34315 15.182C9.22833 18.0672 13.769 18.2879 16.9075 15.8442C16.921 15.8595 16.9351 15.8745 16.9497 15.8891L21.1924 20.1317C21.5829 20.5223 22.2161 20.5223 22.6066 20.1317C22.9971 19.7412 22.9971 19.1081 22.6066 18.7175L18.364 14.4749C18.3493 14.4603 18.3343 14.4462 18.319 14.4326ZM16.2426 5.28251C18.5858 7.62565 18.5858 11.4246 16.2426 13.7678C13.8995 16.1109 10.1005 16.1109 7.75736 13.7678C5.41421 11.4246 5.41421 7.62565 7.75736 5.28251C10.1005 2.93936 13.8995 2.93936 16.2426 5.28251Z"
					fill="currentColor"
				/>
			</svg></button
		>
	</div>

	<div>
		<button class="formButton filterButton"
			>Filter<svg
				width="24"
				height="24"
				viewBox="0 0 24 24"
				fill="none"
				xmlns="http://www.w3.org/2000/svg"
			>
				<path
					d="M5 7.41421L6.41421 6L12.0711 11.6569L17.7279 6L19.1421 7.41421L12.0711 14.4853L5 7.41421Z"
					fill="currentColor"
				/>
				<path d="M19 16.3432H5V18.3432H19V16.3432Z" fill="currentColor" />
			</svg></button
		>
	</div>
</div>

<form class="form">
	<fieldset>
		<legend>Cultural Tribe</legend>

		<input type="checkbox" id="silkroad" name="monster" value="K" />
		<label for="silkroad">Silkroad</label><br />

		<input type="checkbox" id="modern" name="monster" value="S" />
		<label for="modern">Modern Times</label><br />

		<input type="checkbox" id="golden" name="monster" value="M" />
		<label for="golden">Golden Age</label>
	</fieldset>
	<fieldset>
		<legend>Size and Dimensions</legend>

		<input type="checkbox" id="10cm" name="monster" value="K" />
		<label for="10cm">0cm - 10cm</label><br />

		<input type="checkbox" id="20cm" name="monster" value="S" />
		<label for="20cm">10cm - 20cm</label><br />

		<input type="checkbox" id="30cm" name="monster" value="M" />
		<label for="30cm">20cm - 30cm</label><br />

		<input type="checkbox" id="50cm" name="monster" value="M" />
		<label for="30cm">30cm - 50cm</label>
	</fieldset>
	<fieldset>
		<legend>Material technique</legend>

		<input type="checkbox" id="weaving" name="monster" value="K" />
		<label for="weaving">Weaving</label><br />

		<input type="checkbox" id="forging" name="monster" value="S" />
		<label for="forging">Forging</label><br />

		<input type="checkbox" id="sculpturing" name="monster" value="M" />
		<label for="sculpturing">Sculpturing</label><br />

		<input type="checkbox" id="electronics" name="monster" value="M" />
		<label for="electronics">Electronics</label>
	</fieldset>
	<fieldset>
		<legend>Location found</legend>

		<input type="checkbox" id="damrak" name="monster" value="K" />
		<label for="damrak">Damrak</label><br />

		<input type="checkbox" id="rokin" name="monster" value="S" />
		<label for="rokin">Rokin</label><br />
	</fieldset>
</form>

<style>
	form {
		opacity: 0;
		display: flex;
		justify-content: space-between;
		padding: 2em 10vw;
		font-size: 1.3em;
		background: #f3f1ed;
	}

	fieldset legend {
		font-weight: 700;
	}

	.subfilter {
		display: flex;
		justify-content: space-between;
		padding: 2em 10vw;
		background: #f3f1ed;
	}

	[type='search'] {
		background: white;
		padding: 10px 40px;
		border-top: none;
		border-right: none;
		border-left: none;
	}

	.formButton {
		background: var(--secondary-color);
		padding: 10px 40px;
		font-weight: 700;
		color: #e1e1e1;
		width: max-content;
		font-family: 'IBM Plex Mono', monospace;
		transition: all 250ms ease;
		border: none;
		display: flex;
	}

	.formButton svg {
		margin-left: 1.5em;
	}

	.search {
		display: flex;
	}
</style>
