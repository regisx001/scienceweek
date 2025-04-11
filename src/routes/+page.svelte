<script lang="ts">
	import { EventCards } from '$lib/components/ui/cards/index.js';
	import { SponsorsCards } from '$lib/components/ui/MagicCard/index.js';
	import { Number } from '$lib/components/ui/Numbers/index.js';
	import { Overview } from '$lib/components/ui/Overview/index.js';
	import { TimeLineExample } from '$lib/components/ui/Timeline/index.js';
</script>

<svelte:head>
	<title>Science Week | Explorez l'Avenir de la Science</title>
</svelte:head>

<EventCards />

<TimeLineExample />
<Number />

<Overview />

<div class="h-44"></div>
<SponsorsCards />
