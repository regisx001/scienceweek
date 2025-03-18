<script lang="ts">
	import '../app.css';
	import { ModeWatcher } from 'mode-watcher';
	import {
		NavbarMenu,
		HoveredLink,
		MenuItem,
		ProductItem
	} from '$lib/components/ui/NavbarMenu/index.js';

	import { Footer } from '$lib/components/ui/Footer/index.js';
	import { base } from '$app/paths';
	import ShineBorder from '$lib/components/ui/ShineBorder.svelte';
	let active: string | null = null;
	let { children } = $props();
	// Navbar related
	let { visible } = $state(true);
	let lastScroll = $state(0);

	$effect(() => {
		const handleScroll = () => {
			const currentScroll = window.scrollY;
			const scrollingDown = currentScroll > lastScroll && currentScroll > 100;

			visible = !scrollingDown;
			lastScroll = currentScroll;
		};

		// Throttle scroll events
		const throttledScroll = throttle(handleScroll, 100);
		window.addEventListener('scroll', throttledScroll);

		return () => window.removeEventListener('scroll', throttledScroll);
	});

	function throttle(fn, wait) {
		let time = Date.now();
		return () => {
			if (time + wait - Date.now() < 0) {
				fn();
				time = Date.now();
			}
		};
	}
</script>

<ModeWatcher track={false} defaultMode={'dark'} />

<nav
	class="fixed left-0 right-0 top-0 z-50 mx-[10%] my-4 flex h-16 items-center justify-between rounded-full border-b border-border bg-background/95 px-6 backdrop-blur-lg transition-all duration-300"
	style:transform={visible ? 'translateY(0)' : 'translateY(-100%)'}
	style:opacity={visible ? '1' : '0'}
>
	<!-- Logo -->
	<div class="flex items-center gap-2">
		<svg
			class="h-8 w-8 text-primary"
			fill="none"
			stroke="currentColor"
			stroke-width="1.5"
			viewBox="0 0 24 24"
		>
			<path
				stroke-linecap="round"
				stroke-linejoin="round"
				d="M15.59 14.37a6 6 0 01-5.84 7.38v-4.8m5.84-2.58a14.98 14.98 0 006.16-12.12A14.98 14.98 0 009.631 8.41m5.96 5.96a14.926 14.926 0 01-5.841 2.58m-.119-8.54a6 6 0 00-7.381 5.84h4.8m2.581-5.84a14.927 14.927 0 00-2.58 5.84m2.699 2.7c-.103.021-.207.041-.311.06a15.09 15.09 0 01-2.448-2.448 14.9 14.9 0 01.06-.312m-2.24 2.39a4.493 4.493 0 00-1.757 4.306 4.493 4.493 0 004.306-1.758M16.5 9a1.5 1.5 0 11-3 0 1.5 1.5 0 013 0z"
			/>
		</svg>
		<span class="text-lg font-semibold text-foreground">ScienceWeek</span>
	</div>

	<!-- Navigation Links -->
	<div class="hidden items-center gap-6 md:flex">
		<a
			href="#program"
			class="text-sm font-medium text-muted-foreground transition-colors hover:text-foreground"
		>
			Program
		</a>
		<a
			href="#speakers"
			class="text-sm font-medium text-muted-foreground transition-colors hover:text-foreground"
		>
			Speakers
		</a>
		<a
			href="#register"
			class="rounded-full bg-primary px-4 py-2 text-sm font-medium text-primary-foreground shadow-sm transition-colors hover:bg-primary/90"
		>
			Register Now
		</a>
	</div>

	<!-- Mobile Menu -->
	<button class="text-muted-foreground md:hidden">
		<svg class="h-6 w-6" fill="none" stroke="currentColor" stroke-width="1.5" viewBox="0 0 24 24">
			<path
				stroke-linecap="round"
				stroke-linejoin="round"
				d="M3.75 6.75h16.5M3.75 12h16.5m-16.5 5.25h16.5"
			/>
		</svg>
	</button>
</nav>
<!-- <div class="relative flex w-full items-center justify-center">
	<div class={'fixed inset-x-0 top-8 z-50 mx-auto max-w-2xl'}>
		<NavbarMenu>
			<a href="{base}/" class="font-bold text-neutral-700 hover:text-black dark:text-neutral-200">
				Home
			</a><a
				href="{base}/program"
				class=" font-bold text-neutral-700 hover:text-black dark:text-neutral-200"
			>
				Programme
			</a>
		</NavbarMenu>
	</div>
</div> -->
<main class="relative mt-72 lg:mt-44">
	{@render children()}
</main>
<Footer />

<style>
	nav {
		box-shadow: 0 4px 30px rgba(0, 0, 0, 0.25);
		transition:
			transform 0.3s cubic-bezier(0.4, 0, 0.2, 1),
			opacity 0.2s ease-in-out;
	}
</style>
