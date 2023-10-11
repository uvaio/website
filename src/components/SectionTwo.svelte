<script>
	import HorizontalBar from '../components/HorizontalBar.svelte';
</script>

<section class="lazyload">
	<img class="ornamentOne" src="/images/object-1.png" />
	<h1>Time of Origin</h1>
	<p>
		During the excavation items from many different time frames where found. This section displays
		how many items where found at what <em>time period</em> roughly in centuries.
	</p>
	<HorizontalBar />
</section>

<style>
	.ornamentOne {
		position: absolute;
		transform: translateY(-15em) translateX(-10em) scale(1.3);
	}
</style>
