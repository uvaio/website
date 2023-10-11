<script>
	import { onMount } from 'svelte';
	import Chart from 'chart.js/auto';

	onMount(async () => {
		Chart.defaults.font.family = 'IBM Plex Mono';
		Chart.defaults.backgroundColor = '#9BD0F5';
		Chart.defaults.color = '#000';

		const ctx = document.getElementById('Polar');

		new Chart(ctx, {
			type: 'polarArea',
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
			options: {}
		});
	});
</script>

<article>
	<canvas id="Polar" />
</article>
