<script>
	import { cn } from '$lib/utils.js';

	let card = {
		title: 'Hello Developers',
		desc: 'Life is good when you are a developer.'
	};
	let className = 'p-8 dark:bg-zinc-900/30';
	export { className as class };
</script>

<div>
	<div
		class="relative h-full border-[0.5px] border-zinc-400 shadow-[4px_4px_0px_0px_rgba(0,0,0)] dark:border-white/70 dark:shadow-[3px_3px_0px_0px_rgba(255,255,255,0.7)]"
	>
		<slot />
	</div>
</div>
