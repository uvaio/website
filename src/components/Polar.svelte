<script>
	import { onMount } from 'svelte';
	import Chart from 'chart.js/auto';

	import { categories } from '../data/categories';

	onMount(async () => {
		Chart.defaults.font.family = 'IBM Plex Mono';
		Chart.defaults.backgroundColor = '#9BD0F5';
		Chart.defaults.color = '#000';

		const ctx = document.getElementById('Polar');

		let labels = [];
		let amount = [];

		for (let item of categories) {
			labels.push(item.category);
		}

		for (let item of categories) {
			amount.push(item.amount);
		}

		console.log(categories);
		console.log(labels);
		console.log(amount);

		new Chart(ctx, {
			type: 'polarArea',
			data: {
				labels: labels,
				datasets: [
					{
						data: amount
					}
				]
			},
			options: { maintainAspectRatio: true, responsive: true }
		});
	});
</script>

<article>
	<canvas id="Polar" />
</article>

<style>
	article {
		width: 100vw;
		height: 60vh;
	}
</style>
