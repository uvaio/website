<script>
	import Polar from '../components/Polar.svelte';
</script>

<section class="lazyload">
	<img class="ornamentTwo" src="/images/object-2.png" />
	<h1 id="functional">Functional properties</h1>
	<p>
		The objects are categorized by <strong>functional property</strong> which means the intentional
		use of the object. Bowls, plates and dishes that were found are categorized as
		<em>Food Processing</em> and Axes, Hooks are categorized as <em>Craft & Industry</em>.
	</p>
	<Polar />s
</section>

<style>
	.ornamentTwo {
		position: absolute;
		right: 0;
		transform: translateY(-15em) translateX(1em) scale(1.5) rotate(30deg);
	}
</style>
