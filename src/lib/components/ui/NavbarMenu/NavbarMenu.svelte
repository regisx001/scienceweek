<script>
	import ShineBorder from '../ShineBorder.svelte';
</script>

<ShineBorder class="w-full rounded-full" color="white">
	<!-- <nav
		class="boder relative flex justify-center gap-4 space-x-4 rounded-full bg-black px-8 py-4 shadow-input dark:border-white/[0.2]"
	>
		<slot />
	</nav> -->
	<nav
		class="relative flex justify-center gap-4 space-x-4 rounded-full bg-black px-8 py-2 shadow-[0_0_15px_rgba(255,255,255,0.05)] dark:border-white/[0.2]"
	>
		<slot />
	</nav>
</ShineBorder>
