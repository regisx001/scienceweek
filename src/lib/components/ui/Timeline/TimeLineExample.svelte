<script>
	import Timeline from './Timeline.svelte';
	import Day01 from './Day01.svelte';
	import Day02 from './Day02.svelte';
	import Day03 from './Day03.svelte';
	import Day04 from './Day04.svelte';
	import Day05 from './Day05.svelte';
	import Day06 from './Day06.svelte';

	let timelineData = [
		{
			title: "Journée 1: Cérémonie d'ouverture",
			content: Day01
		},
		{
			title: 'Journée 2: Informatique',
			content: Day02
		},
		{
			title: 'Journée 3: Mécanique',
			content: Day03
		},
		{
			title: 'Journée 4: Électrique',
			content: Day04
		},
		{
			title: 'Journée 5: Entrepreneuriat',
			content: Day05
		},
		{
			title: 'Journée 6: Clôture & Galerie',
			content: Day06
		}
	];
</script>

<Timeline {timelineData} />
