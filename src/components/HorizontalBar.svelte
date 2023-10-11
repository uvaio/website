<script>
	import { onMount } from 'svelte';
	import Chart from 'chart.js/auto';

	onMount(async () => {
		Chart.defaults.font.family = 'IBM Plex Mono';
		Chart.defaults.backgroundColor = '#9BD0F5';
		Chart.defaults.color = '#000';

		const ctx = document.getElementById('HorizontalBar');

		new Chart(ctx, {
			type: 'bar',
			data: {
				labels: ['1700-1800', '1800', '1900', '2000'],
				datasets: [
					{
						label: '# of Votes',
						data: [12, 19, 3, 5, 2, 3],
						borderWidth: 2,
						backgroundColor: '#656565'
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
				plugins: {}
			}
		});
	});
</script>

<article>
	<canvas id="HorizontalBar" />
</article>
