<script>
	import { onMount } from 'svelte';
	import Chart from 'chart.js/auto';

	import { years } from '../data/years';

	onMount(async () => {
		Chart.defaults.font.family = 'IBM Plex Mono';
		Chart.defaults.backgroundColor = '#9BD0F5';
		Chart.defaults.backgroundColor = '#000';
		Chart.defaults.color = '#000';

		const ctx = document.getElementById('Bar');

		let labels = [];
		let amount = [];

		for (let item of years) {
			labels.push(item.years);
		}

		for (let item of years) {
			amount.push(item.amount);
		}

		console.log(years);
		console.log(labels);
		console.log(amount);

		new Chart(ctx, {
			type: 'bar',
			data: {
				labels: labels,
				datasets: [
					{
						data: amount,
						backgroundColor: '#000'
					}
				]
			},
			options: {
				indexAxis: 'y',
				// Elements options apply to all of the options unless overridden in a dataset
				// In this case, we are setting the border of each horizontal bar to be 2px wide
				elements: {
					bar: {
						borderWidth: 2
					}
				},
				responsive: true,
				plugins: {
					legend: {
						display: false
					}
				}
			}
		});
	});
</script>

<article>
	<canvas id="Bar" />
</article>
