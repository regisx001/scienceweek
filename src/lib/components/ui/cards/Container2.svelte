<script>
	import Line from './Line.svelte';
</script>

<div class="relative mx-auto w-fit px-4 sm:px-6 md:px-8">
	<Line class="left-0 top-2 bg-gradient-to-l sm:top-4 md:top-6" />
	<Line class="bottom-2 left-0 bg-gradient-to-r sm:bottom-4 md:bottom-6" />

	<Line class="inset-y-0 right-2 h-full w-px bg-gradient-to-t sm:right-4 md:right-6" />
	<Line class="inset-y-0 left-2 h-full w-px bg-gradient-to-t sm:left-4 md:left-6" />
	<div class="relative z-20 mx-auto py-8">
		<slot></slot>
	</div>
</div>
