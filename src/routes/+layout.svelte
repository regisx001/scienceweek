<script lang="ts">
	import '../app.css';
	import { ModeWatcher } from 'mode-watcher';

	import { Footer } from '$lib/components/ui/Footer/index.js';
	import { Navbar } from '$lib/components/ui/Navbar/index.js';
	let active: string | null = null;
	let { children } = $props();
	// Navbar related
</script>

<ModeWatcher track={false} defaultMode={'dark'} />
<Navbar />

<main class="relative mt-72 lg:mt-44">
	{@render children()}
</main>
<Footer />
