<aside>
	<nav>
		<ol>
			<li>Function of objects</li>
			<li>Country of Origin</li>
			<li>Material Types</li>
			<li>Material Types</li>
			<li>Material Types</li>
		</ol>
	</nav>
	<button>Sections</button>
</aside>

<style>
	aside {
		position: fixed;
		left: 0;
		top: 10vh;
		background: var(--secondary-color);
		color: var(--primary-color);
		width: 20vw;
		padding: 1em;
		transform: translateX(-85%);
		transition: all 250ms ease;
	}

	aside button {
		position: absolute;
		right: -0.2em;
		top: 38%;
		transform: rotate(90deg);
		background: none;
		color: var(--primary-color);
		border: none;
		text-transform: uppercase;
		font-weight: bold;
		padding-bottom: 2em;
		border-bottom: 1px solid white;
	}

	aside:hover {
		transform: translateX(0%);
	}
</style>
