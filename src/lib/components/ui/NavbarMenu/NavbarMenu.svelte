<script>
	import ShineBorder from '../ShineBorder.svelte';
</script>

<ShineBorder class="w-full rounded-full" color="white">
	<nav
		class="boder relative flex justify-center gap-4 space-x-4 rounded-full bg-black px-8 py-4 shadow-input dark:border-white/[0.2]"
	>
		<slot />
	</nav>
</ShineBorder>
