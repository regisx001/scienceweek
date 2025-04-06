<script>
	import Timeline from './Timeline.svelte';
	import Day01 from './Day01.svelte';
	import Day02 from './Day02.svelte';
	import Day03 from './Day03.svelte';
	import Day04 from './Day04.svelte';
	import Day05 from './Day05.svelte';
	import Ouverture from './ouverture.svelte';
	import Mecanique from './mecanique.svelte';
	import Ecomnomie from './ecomnomie.svelte';
	import Informatique from './informatique.svelte';
	import Cloture from './cloture.svelte';

	let timelineData = [
		{
			title: "Journée 1: Cérémonie d'ouverture & Electrique",
			content: Ouverture
		},
		{
			title: 'Journée 2: Mécanique',
			content: Mecanique
		},
		{
			title: 'Journée 3: Entrepreneuriat et Economie',
			content: Ecomnomie
		},
		{
			title: 'Journée 4: Informatique',
			content: Informatique
		},
		{
			title: 'Journée 5: Clôture & Galerie',
			content: Cloture
		}
	];
</script>

<Timeline {timelineData} />
