<script lang="ts">
	import { base } from '$app/paths';

	let visible = $state(true);
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

	function throttle(fn: { (): void; (): void }, wait: number) {
		let time = Date.now();
		return () => {
			if (time + wait - Date.now() < 0) {
				fn();
				time = Date.now();
			}
		};
	}
</script>

<nav
	class="fixed left-0 right-0 top-0 z-50 mx-[10%] my-4 flex h-16 items-center justify-between rounded-full border-b border-border bg-background/95 px-6 backdrop-blur-lg transition-all duration-300"
	style:transform={visible ? 'translateY(0)' : 'translateY(-100%)'}
	style:opacity={visible ? '1' : '0'}
>
	<!-- Logo -->
	<a href="{base}/">
		<div class="relative flex items-center gap-2">
			<div class="absolute h-8 w-8 rounded bg-white lg:h-14 lg:w-14 lg:rounded-xl"></div>
			<img class="z-10 w-8 rounded-full lg:w-14" src="{base}/favicon.png" alt="" srcset="" />
			<span class="font-serif text-sm font-semibold text-foreground lg:text-2xl">
				The Legends Club | Science Week
			</span>
		</div>
	</a>

	<!-- Navigation Links -->
	<div class="hidden items-center gap-6 md:flex">
		<a
			href="{base}/program"
			class="text-sm font-medium text-muted-foreground transition-colors hover:text-foreground"
		>
			Program
		</a>
		<!-- <a
			href="#speakers"
			class="text-sm font-medium text-muted-foreground transition-colors hover:text-foreground"
		>
			Speakers
		</a> -->
		<a
			href="{base}/register"
			class="rounded-full bg-primary px-4 py-2 text-sm font-medium text-primary-foreground shadow-sm transition-colors hover:bg-primary/90"
		>
			S'inscrire Maintenant
		</a>
	</div>
</nav>

<style>
	nav {
		box-shadow: 0 4px 30px rgba(0, 0, 0, 0.25);
		transition:
			transform 0.3s cubic-bezier(0.4, 0, 0.2, 1),
			opacity 0.2s ease-in-out;
	}
</style>
