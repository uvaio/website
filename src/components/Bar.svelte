<script>
	import { onMount } from 'svelte';
	import Chart from 'chart.js/auto';

	onMount(async () => {
		const ctx = document.getElementById('Bar');

		new Chart(ctx, {
			type: 'bar',
			data: {
				labels: ['Red', 'Blue', 'Yellow', 'Green'],
				datasets: [
					{
						label: '# of Votes',
						data: [12, 19, 3, 5, 2, 3],
						borderWidth: 1
					}
				]
			},
			options: {
				scales: {
					y: {
						beginAtZero: true
					}
				}
			}
		});
	});
</script>

<article>
	<canvas id="Bar" />
</article>
