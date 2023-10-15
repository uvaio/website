<script>
	import { onMount } from 'svelte';
	import Chart from 'chart.js/auto';

	import { materials } from '../data/materials';

	onMount(async () => {
		Chart.defaults.font.family = 'IBM Plex Mono';
		Chart.defaults.backgroundColor = '#9BD0F5';
		Chart.defaults.color = '#000';

		const ctx = document.getElementById('Pie');

		let labels = [];
		let amount = [];

		for (let item of materials) {
			labels.push(item.category);
		}

		for (let item of materials) {
			amount.push(item.amount);
		}

		console.log(materials);
		console.log(labels);
		console.log(amount);

		new Chart(ctx, {
			type: 'doughnut',
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
	<canvas id="Pie" />
</article>
