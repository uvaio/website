<section class="grid">
	<article>
		<img src="/images/objects/object-1.png" />
		<h4>TELEPHONE CARD</h4>
		<h5>NZD1.00303KST002</h5>
	</article>
	<article>
		<img src="/images/objects/object-2.png" />
		<h4>BANK CARD</h4>
		<h5>NZD1.00027KST002</h5>
	</article>
	<article>
		<img src="/images/objects/object-3.png" />
		<h4>MOBILE PHONE</h4>
		<h5>NZD1.00070KST001</h5>
	</article>
	<article>
		<img src="/images/objects/object-4.png" />
		<h4>SUBWAY MAP</h4>
		<h5>NZD1.00021MTL004-01</h5>
	</article>
	<article>
		<img src="/images/objects/object-5.png" />
		<h4>BRONZE STATUE</h4>
		<h5>NZR2.00253CER155</h5>
	</article>
	<article>
		<img src="/images/objects/object-6.png" />
		<h4>SMOKE PIPE</h4>
		<h5>NZR2.00571CER058</h5>
	</article>
	<article>
		<img src="/images/objects/object-7.png" />
		<h4>COIN STAND</h4>
		<h5>NZR2.00197CPY002-01</h5>
	</article>
	<article>
		<img src="/images/objects/object-8.png" />
		<h4>CASETTE</h4>
		<h5>NZD1.00509MTL022</h5>
	</article>
	<article>
		<img src="/images/objects/object-9.png" />
		<h4>MARBLE PIECE</h4>
		<h5>NZD1.00303MTL048</h5>
	</article>
	<article>
		<img src="/images/objects/object-10.png" />
		<h4>DOOR KNOB</h4>
		<h5>NZD1.00096MTL032</h5>
	</article>
	<article>
		<img src="/images/objects/object-11.png" />
		<h4>DOOR SHARD</h4>
		<h5>NZR2.00526MTL032</h5>
	</article>
	<article>
		<img src="/images/objects/object-12.png" />
		<h4>CUP HOLDER</h4>
		<h5>NZV1.00013MTL0102</h5>
	</article>
	<article>
		<img src="/images/objects/object-13.png" />
		<h4>LAMP CONNECTION</h4>
		<h5>NZR2.00509LEE031</h5>
	</article>
	<article>
		<img src="/images/objects/object-14.png" />
		<h4>SMOKE STAND</h4>
		<h5>NZD1.00462MTL162</h5>
	</article>
	<article>
		<img src="/images/objects/object-15.png" />
		<h4>BUCKET HANDLE</h4>
		<h5>NZR2.00418CPY043-01</h5>
	</article>
	<article>
		<img src="/images/objects/object-16.png" />
		<h4>ELECTRIC POLE</h4>
		<h5>NZD1.00366MTL004-04</h5>
	</article>
	<article>
		<img src="/images/objects/object-17.png" />
		<h4>ELECTRIC TRAY</h4>
		<h5>NZR2.00514CER004</h5>
	</article>
	<article>
		<img src="/images/objects/object-18.png" />
		<h4>STATUE PART</h4>
		<h5>NZR2.00115CER075</h5>
	</article>
	<article>
		<img src="/images/objects/object-19.png" />
		<h4>VASE SHARD</h4>
		<h5>NZR2.00223GLS014</h5>
	</article>
	<article>
		<img src="/images/objects/object-20.png" />
		<h4>JUICE VASE</h4>
		<h5>NZR2.00899FAU001-01</h5>
	</article>
</section>

<style>
	.grid {
		display: grid;
		grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
		padding: 3vw 10vw 10vw 10vw;
	}

	article {
		display: flex;
		flex-direction: column;
		align-items: center;
	}

	article img {
		transition: all 250ms ease;
	}

	article h4 {
		margin-bottom: 0;
	}

	article h5 {
		font-weight: 400;
		font-family: 'IBM Plex Mono', monospace;
	}

	article:hover img {
		transform: scale(1.2);
	}
</style>
