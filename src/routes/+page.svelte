<script>
	import Nav from '../components/Nav.svelte';
	import Hero from '../components/Hero.svelte';
	import Timeline from '../components/Timeline.svelte';
	import Projects from '../components/Projects.svelte';
	import Contact from '../components/Contact.svelte';
	import Footer from '../components/Footer.svelte';
	import { onMount } from 'svelte';

	let glowRef;

	const glowSize = 500; // Adjust this value to change the size of the glowing circle

	onMount(() => {
		const handleMouseMove = (e) => {
			const { pageX: x, pageY: y } = e;

			glowRef.style.left = `${x - glowSize / 2}px`;

			glowRef.style.top = `${y - glowSize / 2}px`;
		};

		window.addEventListener('mousemove', handleMouseMove);

		return () => {
			window.removeEventListener('mousemove', handleMouseMove);
		};
	});
</script>

<div class="background-container bg-blue-950">
	<div
		class="glow bg-indigo-500 bg-opacity-10 blur-3xl"
		bind:this={glowRef}
		style="width: {glowSize}px; height: {glowSize}px;"
	></div>

	<div class="content">
		<Nav />

		<Hero />

		<Timeline />

		<Projects />

		<Contact />

		<Footer />
	</div>
</div>

<style>
	.background-container {
		position: relative;

		overflow: hidden;
	}

	.glow {
		position: absolute;

		width: 500px;

		height: 500px;

		border-radius: 50%;

		pointer-events: none;

		transition: transform 0.1s ease-out;

		z-index: 0; /* Ensure it's in the background */
	}

	.content {
		position: relative;

		z-index: 1; /* Ensure content is above the glow effect */
	}
</style>
