<script>
	import Stats from '../components/Stats.svelte';
</script>

<section>
	<h1>Introduction</h1>
	<p>
		Lorem, ipsum dolor sit amet consectetur adipisicing elit. Cupiditate culpa expedita maxime,
		cumque perferendis, libero ullam dolores, laudantium exercitationem sapiente neque ipsum tempore
		perspiciatis. Natus quo numquam quaerat sed neque!
	</p>
	<p>
		Lorem ipsum dolor sit amet consectetur adipisicing elit. Labore eos similique nostrum nesciunt
		dolor expedita quibusdam, distinctio magnam velit dignissimos non suscipit maxime? Eius
		inventore doloribus ratione maxime eligendi odio!
	</p>
	<p>
		Lorem ipsum dolor sit amet consectetur adipisicing elit. Labore eos similique nostrum nesciunt
		dolor expedita quibusdam, distinctio magnam velit dignissimos non suscipit maxime? Eius
		inventore doloribus ratione maxime eligendi odio!
	</p>
	<Stats />
</section>

<style>
	h1,
	p,
	.button {
		opacity: 0;
		animation: left 300ms ease 1s forwards;
	}

	@keyframes left {
		0% {
			transform: translateY(1em);
			opacity: 0;
		}

		100% {
			transform: translateY(0em);
			opacity: 1;
		}
	}
</style>
