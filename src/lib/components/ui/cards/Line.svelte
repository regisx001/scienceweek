<script>
	import { cn } from '$lib/utils.js';

	let className = '';
	export { className as class };
</script>

<div
	class={cn(
		'absolute -z-0 h-px w-full from-zinc-200 from-[1%] via-zinc-400 to-zinc-600 dark:from-zinc-900 dark:via-zinc-700 dark:to-zinc-500',
		className
	)}
></div>
