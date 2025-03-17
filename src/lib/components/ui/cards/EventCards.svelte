<script lang="ts">
	import Container from './Container.svelte';

	let card = {
		title: 'Svelte is Vibe',
		desc: 'Svelte is javascript framework that is easy to learn and use. '
	};
	let className: any = 'p-6';
	export { className as class };
</script>

<header class="relative overflow-hidden pb-32 pt-24">
	<div class="mx-auto grid max-w-7xl items-center gap-16 px-4 lg:grid-cols-2">
		<div class="relative z-10 space-y-8">
			<h1 class="text-5xl font-bold leading-tight md:text-6xl">
				Explorez l'Avenir de la
				<span class="gradient-text">Science</span>
			</h1>
			<p class="max-w-2xl text-xl leading-relaxed text-gray-400">
				Rejoignez 15,000 scientifiques et passionnés pour 6 jours d'innovation, de découvertes
				révolutionnaires et de réseautage international.
			</p>
			<div class="flex flex-wrap gap-4">
				<button
					class="rounded-full bg-transparent px-8 py-4 font-bold uppercase tracking-widest shadow-[inset_0_0_0_2px_#616467] transition duration-200 hover:bg-[#616467] hover:text-white dark:text-neutral-200"
				>
					S'inscrire Maintenant
				</button>

				<button
					class="rounded-full bg-transparent px-8 py-4 font-bold uppercase tracking-widest shadow-[inset_0_0_0_2px_#616467] transition duration-200 hover:bg-[#616467] hover:text-white dark:text-neutral-200"
				>
					Voir le Programme
				</button>
			</div>
		</div>
		<div class="relative">
			<div class="absolute inset-0 -rotate-6 transform rounded-full bg-blue-500/10 blur-3xl"></div>
			<div class="relative grid grid-cols-2 gap-4">
				<div class="col-span-1 space-y-4">
					<Container>
						<div class="aspect-square overflow-hidden rounded-2xl bg-gray-800">
							<img
								src="https://www.wtcmanila.com.ph/wp-content/uploads/2022/08/rear-view-of-audience-in-the-conference-hall-or-se-2021-08-30-06-51-57-utc-1.jpg"
								class="h-full w-full object-cover"
							/>
						</div>
					</Container>
					<Container>
						<div class=" overflow-hidden rounded-2xl bg-gray-800">
							<img
								src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTSINxkBL8YzQbtIa11V7xykxHRocn2uSgBiw&s"
								class="h-full w-full object-cover"
							/>
						</div>
					</Container>
				</div>

				<div class="col-span-1 space-y-4 pt-12">
					<Container>
						<div class=" overflow-hidden rounded-2xl bg-gray-800">
							<img
								src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSxBjQ6cacjUhWGAxXt_j-UgOdQhDAo3ce9Eg&s"
								class="h-full w-full object-cover"
							/>
						</div>
					</Container>
					<Container>
						<div class="aspect-square overflow-hidden rounded-2xl bg-gray-800">
							<img
								src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRDYjkEzAf8K-tqsa-Sy8JCnDk1VPvrVLzzaA&s"
								class="h-full w-full object-cover"
							/>
						</div>
					</Container>
				</div>
			</div>
		</div>
	</div>
</header>
