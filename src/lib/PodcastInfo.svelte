<script lang="ts">

	// Type Imports:
	import type { Links } from '$lib/types';

	// Initializations:
	export let links: Links;
	
</script>

<!-- #################################################################################################### -->

<div class="wrapper">
	<section id="podcastInfo">
		<div id="listen">
			<h2>Check out our podcast:</h2>
			<span class="links">
				<a href="{links.podcast.anchor}" target="_blank"><img src="/icons/anchor.png" alt="Anchor"></a>
				<a href="{links.podcast.spotify}" target="_blank"><img src="/icons/spotify.png" alt="Spotify"></a>
				<a href="{links.podcast.apple}" target="_blank"><img src="/icons/apple.png" alt="Apple"></a>
				<a href="{links.podcast.google}" target="_blank"><img src="/icons/google.png" alt="Google"></a>
			</span>
		</div>
		<div id="info">
			<p>Web3 has rewritten many rules about building products, acquiring users & collaboration. Composability, open data, airdrops, tokens, DAOs - all these things can be confusing even for web3 native people, let alone people who're just entering the space.</p>
			<p>Web3 Talks is a place to learn the nuts & bolts of web3 by listening to the stories of successful web3 projects. <span class="highlight">You can learn what has worked and what hasn't, so you don't repeat their mistakes.</span></p>
			<p>As we're focused on builders, <span class="highlight">we don't talk high-level VC stuff</span> like “What is Metaverse?” or trading-oriented things such as “Which coin should you invest in 2022?”.</p>
			<p>Instead, we focus on questions such as <span class="highlight">“How have you acquired first users?”</span>, <span class="highlight">“How do you take care of your community?”</span> or <span class="highlight">“What were the biggest technical challenges that you've faced so far?”</span></p>
			<p>Our vision is to be a place that inspires fellow hackers & entrepreneurs to build their own web3 projects that will <span class="highlight">define the future of the web.</span></p>
		</div>
	</section>
</div>

<!-- #################################################################################################### -->

<style>

	div.wrapper {
		filter: drop-shadow(0 0 5px var(--primary-color));
	}

	#podcastInfo {
		--sharpness: 20%;
		display: flex;
		gap: 10em;
		margin: -7em 0;
		padding: 10em 10vw;
		background: var(--primary-color);
		-webkit-clip-path: polygon(0 var(--sharpness), 100% 0, 100% calc(100% - var(--sharpness)), 0 100%);
		clip-path: polygon(0 var(--sharpness), 100% 0, 100% calc(100% - var(--sharpness)), 0 100%);
	}

	#podcastInfo > div {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		gap: .5em;
		text-align: center;
		font-size: 1.2em;
	}

	#listen {
		flex: 1;
	}

	h2 {
		font-size: 2em;
		text-shadow: 2px 2px 5px black;
	}

	span.links {
		display: flex;
		gap: 1em;
	}

	span.links > a {
		display: flex;
	}

	span.links > a:hover {
		filter: drop-shadow(0 0 6px var(--accent-color));
	}

	span.links img {
		height: 2em;
		width: 2em;
		border-radius: .5em;
	}

	#info {
		flex: 2;
		text-shadow: 1px 1px 3px black;
	}

	.highlight {
		color: var(--accent-color);
	}
	
</style>