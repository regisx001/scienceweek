<script lang="ts">
	export let showFade: boolean = true;
</script>

<div
	class="bg-grid-black/[0.2] dark:bg-grid-white/[0.2] relative flex h-96 items-center justify-center bg-white dark:bg-black"
>
	<!-- Radial gradient for the container to give a faded look -->
	{#if showFade}
		<div
			class="pointer-events-none absolute inset-0 flex items-center justify-center bg-white [mask-image:radial-gradient(ellipse_at_center,transparent_20%,black)] dark:bg-black"
		></div>
	{/if}
	<slot />
</div>
