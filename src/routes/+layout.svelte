<script>
	import Welcome from "$lib/assets/imgs/welcome.jpg";
  import Footer from "$lib/components/footer/Footer.svelte";
  import Nav from "$lib/components/nav/Nav.svelte";
  import WelcomeMarquee from "$lib/components/welcome-marquee/WelcomeMarquee.svelte";
  import { base } from "$app/paths";
	import "$lib/styles/global.css";

	let { children } = $props();
</script>

<svelte:head>
	<meta name="title" content="vinc3w" />
	<meta name="theme-color" content="#F4ADA0" />
	<meta name="description" content="A retro-style portfolio website for vinc3w.">
	<meta name="keywords" content="vinc3w, portfolio, developer, programmer, web development, software engineering, retro, neocities">
	<meta name="robots" content="index,follow">
	<meta http-equiv="Content-Type" content="text/html; charset=utf-8">
	<meta name="language" content="English">
	<meta name="revisit-after" content="2 days">
	<meta name="author" content="vinc3w">

	<meta property="og:type" content="website" />
	<meta property="og:url" content="https://vinc3w.github.io/retro" />
	<meta property="og:title" content="vinc3w" />
	<meta property="og:description" content="A retro-style portfolio website for vinc3w." />
	<meta property="og:image" content="{base}/avatar.png" />

	<meta property="twitter:card" content="summary_large_image" />
	<meta property="twitter:url" content="https://vinc3w.github.io/retro" />
	<meta property="twitter:title" content="vinc3w" />
	<meta property="twitter:description" content="A retro-style portfolio website for vinc3w." />
	<meta property="twitter:image" content="{base}/avatar.png" />

	<link rel="apple-touch-icon" sizes="180x180" href="{base}/apple-touch-icon.png">
	<link rel="icon" type="image/png" sizes="32x32" href="{base}/favicon-32x32.png">
	<link rel="icon" type="image/png" sizes="16x16" href="{base}/favicon-16x16.png">
	<link rel="manifest" href="{base}/site.webmanifest">
	<title>UwU</title>
</svelte:head>

<div class="content">
	<header>
		<img src={Welcome} alt="welcome" />
	</header>
	<WelcomeMarquee />
	<main>
		<Nav />
		{@render children()}
	</main>
	<Footer />
</div>

<style>
	.content {
		background-color: #FFF;
		border: 1px solid #000;
		border-radius: 8px;
		padding: 4px;
		width: 1000px;
		margin: 0 auto;
	}

	header img {
		width: 100%;
		border: 1px solid #000;
		border-radius: 8px;
		display: block;
	}

	main {
		display: flex;
		gap: 4px;
		margin-top: 4px;
	}
</style>
