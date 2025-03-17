<script lang="ts">
	// import { Home, MessageCircle, User } from '@lucide/svelte';
	import { FloatingNavbar } from '$lib/components/ui/FloatingNavbar/index.js';
	import { BorderBeam } from '$lib/components/ui/BorderBeam/index.js';
	import { SimpleCard1 } from '$lib/components/ui/cards/index.js';
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

<div class="relative flex w-full items-center justify-center">
	<div class={'fixed inset-x-0 top-12 z-50 mx-auto max-w-2xl'}>
		<NavbarMenu>
			<MenuItem {active} item="Services">
				<div class="flex flex-col space-y-4 text-sm">
					<HoveredLink href="#">Web Development</HoveredLink>
					<HoveredLink href="#">Interface Design</HoveredLink>
					<HoveredLink href="#">Search Engine Optimization</HoveredLink>
					<HoveredLink href="#">Branding</HoveredLink>
				</div>
			</MenuItem>
			<MenuItem {active} item="Products">
				<div class="  grid grid-cols-2 gap-10 p-4 text-sm">
					<ProductItem
						title="Algochurn"
						href="#"
						src="https://images.pexels.com/photos/1031659/pexels-photo-1031659.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=2"
						description="Prepare for tech interviews like never before."
					/>
					<ProductItem
						title="Tailwind Master Kit"
						href="#"
						src="https://images.pexels.com/photos/733071/pexels-photo-733071.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=2"
						description="Production ready Tailwind css components for your next project"
					/>
					<ProductItem
						title="Moonbeam"
						href="#"
						src="https://images.pexels.com/photos/730424/pexels-photo-730424.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=2"
						description="Never write from scratch again. Go from idea to blog in minutes."
					/>
					<ProductItem
						title="Rogue"
						href="#"
						src="https://images.pexels.com/photos/745243/pexels-photo-745243.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=2"
						description="Respond to government RFPs, RFIs and RFQs 10x faster using AI"
					/>
				</div>
			</MenuItem>
			<MenuItem {active} item="Pricing">
				<div class="flex flex-col space-y-4 text-sm">
					<HoveredLink href="#">Hobby</HoveredLink>
					<HoveredLink href="#">Individual</HoveredLink>
					<HoveredLink href="#">Team</HoveredLink>
					<HoveredLink href="#">Enterprise</HoveredLink>
				</div>
			</MenuItem>
		</NavbarMenu>
	</div>
	<p class="text-black dark:text-white">The Navbar will show on top of the page</p>
</div>

<GridAndDotBackgrounds>
	<p
		class="relative z-20 bg-gradient-to-b from-neutral-200 to-neutral-500 bg-clip-text py-8 text-4xl font-bold text-transparent sm:text-7xl"
	>
		Welcome to science Week
	</p>
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
