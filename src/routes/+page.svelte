<script lang="ts">
	// import { Home, MessageCircle, User } from '@lucide/svelte';
	import { FloatingNavbar } from '$lib/components/ui/FloatingNavbar/index.js';
	import { BorderBeam } from '$lib/components/ui/BorderBeam/index.js';
	import { SimpleCard1, EventCards } from '$lib/components/ui/cards/index.js';
	import { MarqueeExample } from '$lib/components/ui/Marquee/index.js';
	import {
		NavbarMenu,
		HoveredLink,
		MenuItem,
		ProductItem
	} from '$lib/components/ui/NavbarMenu/index.js';
	let active: string | null = null;
	import {
		GridAndDotBackgrounds,
		DotBackground,
		GridAndDotBackgroundsSmallGrid
	} from '$lib/components/ui/GridAndDotBackground/index.js';
	import {
		GlowingStarsBackgroundCard,
		GlowingStarsDescription,
		GlowingStarsTitle
	} from '$lib/components/ui/GlowingStars/index.js';

	const navItems = [
		{
			name: 'Home',
			link: '/'
			// icon: Home
		},
		{
			name: 'About',
			link: '/'
			// icon: User
		},
		{
			name: 'Contact',
			link: '/'
			// icon: MessageCircle
		}
	];
</script>

<!-- <div class="relative w-full">
	<FloatingNavbar {navItems} />
	<div
		class="relative grid h-full w-full grid-cols-1 rounded-md border border-neutral-200 bg-white dark:border-white/[0.2] dark:bg-black"
	>
		<p class="p-40 text-center text-4xl font-bold text-neutral-600 dark:text-white">
			Scroll back up to reveal Navbar
		</p>
		<div class="bg-grid-black/[0.1] dark:bg-grid-white/[0.2] absolute inset-0" />
	</div>
</div> -->

<GridAndDotBackgrounds>
	<EventCards />
	<!-- <p
		class="relative z-20 bg-gradient-to-b from-neutral-200 to-neutral-500 bg-clip-text py-8 text-4xl font-bold text-transparent sm:text-7xl"
	>
		Welcome to science Week
	</p> -->
</GridAndDotBackgrounds>
<MarqueeExample />

<SimpleCard1 />

<article
	class="relative flex max-w-xl flex-col items-start justify-between rounded-3xl border border-gray-700/70 bg-background p-7"
>
	<BorderBeam size={150} duration={12} />
	<div class="flex items-center gap-x-4 text-xs">
		<time datetime="2020-03-16" class="text-gray-300">June 7, 2024</time>
		<a
			href="https://github.com/SikandarJODD"
			class="relative z-10 rounded-full border border-gray-100 bg-transparent px-3 py-1.5 font-medium text-gray-200"
			>Svelte-Components</a
		>
	</div>
	<div class="group relative">
		<h3 class="mt-3 text-lg font-semibold leading-6 text-gray-200 group-hover:text-gray-50">
			<a href="/">
				<span class="absolute inset-0"></span>
				Animation Svelte
			</a>
		</h3>
		<p class="mt-5 line-clamp-3 text-sm leading-6 text-gray-600">
			Welcome to Svelte Animation website. This website includes Qualtiy Tailwind CSS and Framer
			Motion Components. Inspired from <span class="text-gray-300 underline underline-offset-2"
				>Magic UI</span
			>
			and <span class="text-gray-300 underline underline-offset-2">Luxe</span>
			Componenets.
		</p>
	</div>
	<div class="relative mt-8 flex items-center gap-x-4">
		<img
			src="https://avatars.githubusercontent.com/u/93428946?v=4"
			alt="bhide"
			class="h-10 w-10 rounded-full bg-gray-50"
		/>
		<div class="text-sm leading-5">
			<p class="font-semibold text-white">
				<a href="https://github.com/SikandarJODD">
					<span class="absolute inset-0"></span>
					Sikandar Bhide
				</a>
			</p>
			<p class="text-gray-500">Svelte Developer</p>
		</div>
	</div>
</article>

<GlowingStarsBackgroundCard>
	<GlowingStarsTitle>Svelte</GlowingStarsTitle>
	<div class="flex items-end justify-between">
		<GlowingStarsDescription>
			The power of full-stack to the frontend. Read the release notes.
		</GlowingStarsDescription>
		<div class="flex h-8 w-8 items-center justify-center rounded-full bg-[hsla(0,0%,100%,.1)]">
			<svg
				xmlns="http://www.w3.org/2000/svg"
				fill="none"
				viewBox="0 0 24 24"
				stroke-width="1.5"
				stroke="currentColor"
				class="h-4 w-4 stroke-2 text-white"
			>
				<path
					stroke-linecap="round"
					stroke-linejoin="round"
					d="M17.25 8.25L21 12m0 0l-3.75 3.75M21 12H3"
				/>
			</svg>
		</div>
	</div>
</GlowingStarsBackgroundCard>
<div class="h-screen"></div>
