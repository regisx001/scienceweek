<script lang="ts">
	import { Motion } from 'svelte-motion';
	export let delay: number;
</script>

<Motion
	let:motion
	initial={{
		opacity: 0
	}}
	animate={{
		opacity: 1
	}}
	transition={{
		duration: 2,
		ease: 'easeInOut',
		delay: delay
	}}
	exit={{
		opacity: 0
	}}
>
	<div
		use:motion
		class="absolute left-1/2 z-10 h-[4px] w-[4px] -translate-x-1/2 rounded-full bg-blue-500 shadow-2xl shadow-blue-400 blur-[1px]"
	/>
</Motion>
