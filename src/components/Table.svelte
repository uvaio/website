<script>
	import { onMount } from 'svelte';

	onMount(async () => {
		const button = document.querySelector('.menu');
		const aside = document.querySelector('aside ol');

		button.addEventListener('click', menu);

		function menu() {
			aside.classList.toggle('open');
		}
	});
</script>

<aside>
	<nav>
		<ol>
			<li><a href="#introduction">Introduction</a></li>
			<li><a href="#time">Time of Origin</a></li>
			<li><a href="#functional">Functional Properties</a></li>
			<li><a href="#material">Material Usage</a></li>
		</ol>
	</nav>
</aside>
<button class="button menu"
	><svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
		<path
			d="M4 6C4 5.44772 4.44772 5 5 5H19C19.5523 5 20 5.44772 20 6C20 6.55228 19.5523 7 19 7H5C4.44772 7 4 6.55228 4 6Z"
			fill="currentColor"
		/>
		<path
			d="M4 18C4 17.4477 4.44772 17 5 17H19C19.5523 17 20 17.4477 20 18C20 18.5523 19.5523 19 19 19H5C4.44772 19 4 18.5523 4 18Z"
			fill="currentColor"
		/>
		<path
			d="M5 11C4.44772 11 4 11.4477 4 12C4 12.5523 4.44772 13 5 13H13C13.5523 13 14 12.5523 14 12C14 11.4477 13.5523 11 13 11H5Z"
			fill="currentColor"
		/>
	</svg></button
>

<style>
	button {
		border: none;
		text-transform: uppercase;
		font-size: 16px;
		position: fixed;
		top: 2vw;
		left: 2vw;
		z-index: 2;
	}

	button svg {
		margin-left: 0;
	}

	aside ol {
		display: flex;
		justify-content: space-between;
		background: var(--secondary-color);
		color: var(--primary-color);
		position: fixed;
		top: 1vw;
		left: 6vw;
		padding: 22px 24px;
		z-index: 2;
		width: 40vw;
		opacity: 0;
		transition: all 250ms ease;
	}

	aside ol li a {
		color: var(--primary-color);
		opacity: 0.8;
		transition: all 250ms ease;
	}

	aside ol li a:hover {
		opacity: 1;
	}

	.menu {
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
