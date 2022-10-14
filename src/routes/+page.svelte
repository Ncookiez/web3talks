<script lang="ts">

	// Imports:
	import Intro from '$lib/Intro.svelte';
	import Socials from '$lib/Socials.svelte';
	import PodcastInfo from '$lib/PodcastInfo.svelte';

	// Type Imports:
	import type { Links } from '$lib/types';

	// Links:
	const links: Links = {
		podcast: {
			anchor: 'https://anchor.fm/web3-talks',
			spotify: 'https://open.spotify.com/show/6xvZbubp8hXCxLhsbvhldh',
			apple: 'https://podcasts.apple.com/us/podcast/web3-talks-stories-tips-from-the-builders/id1595653866',
			google: 'https://podcasts.google.com/feed/aHR0cHM6Ly9hbmNob3IuZm0vcy83Mzc3MTVjOC9wb2RjYXN0L3Jzcw'
		},
		twitter: 'https://twitter.com/web3talks',
		discord: 'https://discord.gg/s5swazxG2D',
		gitcoin: 'https://gitcoin.co/grants/7405/web3-talks-stories-tips-from-the-builders'
	}
	
</script>

<!-- #################################################################################################### -->

<!-- SvelteKit Dynamic Header -->
<svelte:head>
	<title>Web3 Talks</title>
	<meta name="description" content="Learn how to build web3 projects directly from successful web3 builders." />
</svelte:head>

<!-- Intro Header -->
<Intro />

<!-- Podcast Info -->
<PodcastInfo {links} />

<!-- Links -->
<Socials {links} />