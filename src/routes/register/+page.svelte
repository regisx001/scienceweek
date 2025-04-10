<script lang="ts">
	import { Workshop } from '$lib/components/ui/workshop/index.js';

	let data: WorkshopProps[] = [
		{
			title: '⚡ Atelier Électrique : Robot Foot – Jouez avec des robots footballeurs !',
			description:
				"Entrez dans l’univers fascinant de la robotique appliquée au sport ! Cet atelier vous permet de programmer et contrôler des robots qui s'affrontent dans un match de football. Animé par des passionnés de robotique, c’est l’occasion d’apprendre en jouant !",
			date: '14 Avril 2025',
			horaire: '13:30h - 16h',
			lieu: 'Code 212 Ensa ,Tanger',
			link: 'https://docs.google.com/forms/d/e/1FAIpQLSd8qfz0YDvMs1FXJJVD4w49WhGljvCawhMU-VjcPtyNo05mGQ/viewform'
		},
		{
			title: '🛠️ Atelier Mécanique : Impression 3D – Crée ton prototype',
			description:
				"Découvrez les bases de l’impression 3D et réalisez un prototype personnalisé. L'atelier vous initie aux logiciels de modélisation, à la logique de fabrication additive et à la gestion d'une imprimante 3D. Une activité pour les créateurs et futurs ingénieurs du concret !",
			date: '15 Avril 2025',
			horaire: '13:30h - 16h',
			lieu: 'Code 212 Ensa ,Tanger',
			link: 'https://docs.google.com/forms/d/e/1FAIpQLSeZ7PW1cWs7lYrUtTKoya5kM8twKubZ2nk6XxcGkSHeGUmszw/viewform?usp=dialog'
		},
		{
			title: 'Compétition entrepreneuriale — LEGENDS Science Week 2025',
			description:
				'Dans le cadre de la Journée Entrepreneuriat de la Science Week (16 avril 2025), le Club Legends organise un Compétition entrepreneuriale destiné à faire émerger des idées innovantes, concrètes et à fort impact.  Les participants auront une journée pour former une équipe, concevoir un projet, travailler sur un prototype ou business model, et le présenter devant un jury.',
			date: '16 Avril 2025',
			horaire: '12:30h - 16h',
			lieu: 'Code 212 Ensa ,Tanger',
			link: 'https://docs.google.com/forms/d/e/1FAIpQLSecmmJ2dfWleyY2L0X64vjfi1KDMCsm9U4k0F2vZayU8J-U0A/viewform'
		},
		{
			title: 'Atelier Informatique : Épilepsie et Deep Learning',
			description:
				"🔬 Cet atelier vise à explorer l'application du Deep Learning dans la détection et l'analyse des crises d'épilepsie. Nous aborderons les bases du Machine Learning, l'analyse des signaux EEG et les modèles d'apprentissage profond adaptés à la reconnaissance des crises ",
			date: '17 Avril 2025',
			horaire: '13:30h - 16h',
			lieu: 'Code 212 Ensa ,Tanger',
			link: 'https://docs.google.com/forms/d/e/1FAIpQLSfGHw8m9cQ1H5d6ta6FWtIqadZxF__f1AX1Bn9UlozhkzGosg/viewform?usp=dialog'
		},
		{
			title: 'Compétition Artistique – Science Week 2025',
			description:
				'Exprime ta créativité à travers une œuvre originale autour d’un thème librement inspiré de la science, de l’innovation ou de ton univers personnel.   Les œuvres sélectionnées seront exposées lors de la journée de clôture, le 18 avril 2025, et soumises au vote du public.',
			date: '18 Avril 2025',
			horaire: '10h - 13h30',
			lieu: 'Code 212 Ensa ,Tanger',
			link: 'https://docs.google.com/forms/d/e/1FAIpQLSfTD6C39V6Th3h6B4yskVah26mAL28HHdmiFVcXAP7jh4pSZw/viewform'
		}
	];
</script>

<svelte:head>
	<title>Science Week | Inscrivez vous maintenant</title>
</svelte:head>

<div class="h-44"></div>
<div class="mx-auto max-w-7xl">
	<!-- Header -->
	<div class="mb-12 text-center">
		<h1 class="mb-2 text-3xl font-bold text-slate-100">Ateliers à venir</h1>
		<p class="text-slate-400">Parcourez et inscrivez-vous à nos ateliers techniques</p>
	</div>

	<!-- Cards Grid -->
	<div class="grid grid-cols-1 gap-6 md:grid-cols-2 lg:grid-cols-1">
		<!-- Workshop Card 1 -->

		{#each data as workshop, id}
			<Workshop {...workshop} />
			{#if data.length - 1 !== id}
				<div class="flex h-20 items-center justify-center">
					<hr class="h-4 w-32 rotate-90 border bg-slate-800" />
				</div>
			{/if}
		{/each}
	</div>
</div>

<div class="h-44"></div>
