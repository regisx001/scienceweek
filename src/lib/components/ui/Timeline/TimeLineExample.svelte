<script>
	import Timeline from './Timeline.svelte';
	import Day01 from './Day01.svelte';
	import Day02 from './Day02.svelte';
	import Day03 from './Day03.svelte';
	import Day04 from './Day04.svelte';
	import Day05 from './Day05.svelte';

	let timelineData = [
		{
			title: "Journée 1: Cérémonie d'ouverture & Informatique",
			content: Day01
		},
		{
			title: 'Journée 2: Mécanique',
			content: Day02
		},
		{
			title: 'Journée 3: Électrique',
			content: Day03
		},
		{
			title: 'Journée 4: Entrepreneuriat',
			content: Day04
		},
		{
			title: 'Journée 5: Clôture & Galerie',
			content: Day05
		}
	];
</script>

<Timeline {timelineData} />
