<script>
	import Doughnut from '../components/Doughnut.svelte';
</script>

<section class="lazyload">
	<img class="ornamentThree" src="/images/object-3.png" />
	<h1>Material Usage</h1>
	<p>
		What type of <strong>material</strong> the object is made of with all subcategories but they can
		be defined in four broad categories, <em>textiles, alloys, ceramics and food</em>.
	</p>
	<Doughnut />
</section>

<style>
	.ornamentThree {
		position: absolute;
		left: 0;
		transform: translateY(-15em) translateX(-2em) scale(1.5) rotate(-30deg);
	}
</style>
