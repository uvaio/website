<header>
	<h1>Above the Surface</h1>
	<h2>THE ARCHAEOLOGICAL FINDS OF THE NORTH / SOUTHLINE</h2>
	<a class="button" href="#time"
		>Explore the dataset<svg
			class="down"
			width="24"
			height="24"
			viewBox="0 0 24 24"
			fill="none"
			xmlns="http://www.w3.org/2000/svg"
		>
			<path
				d="M11.0001 3.67157L13.0001 3.67157L13.0001 16.4999L16.2426 13.2574L17.6568 14.6716L12 20.3284L6.34314 14.6716L7.75735 13.2574L11.0001 16.5001L11.0001 3.67157Z"
				fill="currentColor"
			/>
		</svg></a
	>

	<div>
		<img src="/images/objects.png" />
	</div>
</header>

<style>
	header {
		height: 60vh;
		display: flex;
		justify-content: center;
		flex-direction: column;
		padding-left: 10vw;
		text-transform: uppercase;
		overflow: hidden;
	}
	header h1 {
		margin: 0;
	}

	header img {
		position: absolute;
		z-index: -1;
		transform: translateX(40em) rotate(5deg) translateY(-30em);
	}

	header div {
		position: relative;
	}

	header h1,
	h2,
	.button {
		animation: left 300ms ease;
	}

	@keyframes left {
		0% {
			transform: translateX(-1em);
			opacity: 0;
		}

		100% {
			transform: translateX(0em);
			opacity: 1;
		}
	}
</style>
