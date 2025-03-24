<script lang="ts">
	import '../app.css';
	import { ModeWatcher, setMode } from 'mode-watcher';

	import { Footer } from '$lib/components/ui/Footer/index.js';
	import { Navbar } from '$lib/components/ui/Navbar/index.js';
	import { onMount } from 'svelte';
	let active: string | null = null;
	let { children } = $props();
	onMount(() => {
		setMode('dark');
	});
	// Navbar related
</script>

<ModeWatcher track={false} defaultMode={'dark'} />
<Navbar />

<main class="relative">
	{@render children()}
</main>
<Footer />
