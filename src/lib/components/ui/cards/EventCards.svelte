<script lang="ts">
	import { TextGenerateEffect } from '../TextGenerateEffect/index.js';
	import Container from './Container.svelte';

	let card = {
		title: 'Svelte is Vibe',
		desc: 'Svelte is javascript framework that is easy to learn and use. '
	};
	// svelte-ignore export_let_unused
	let className = 'p-6';
	export { className as class };
	const text =
		"Rejoignez 15,000 scientifiques et passionnés pour 6 jours d'innovation, de découvertes révolutionnaires et de réseautage international.";
</script>

<div
	class="relative mb-96 flex h-96 items-center justify-center bg-white pt-96 bg-grid-black/[0.2] dark:bg-black dark:bg-grid-white/[0.2]"
>
	<div
		class="pointer-events-none absolute inset-0 flex items-center justify-center bg-white [mask-image:radial-gradient(ellipse_at_center,transparent_20%,black)] dark:bg-black"
	></div>

	<header class="relative overflow-hidden pb-32">
		<div class="grid items-center gap-16 px-4 lg:mx-[10%] lg:grid-cols-3">
			<div class="relative z-10 col-span-3 max-w-full space-y-8 lg:col-span-1">
				<h1 class="text-5xl font-bold leading-tight md:text-6xl">
					Explorez l'Avenir de la
					<span class="gradient-text">Science</span>
				</h1>

				<TextGenerateEffect className=" text-gray-400" words={text} />
				<!-- <p class="max-w-2xl text-xl leading-relaxed text-gray-400">
				Rejoignez 15,000 scientifiques et passionnés pour 6 jours d'innovation, de découvertes révolutionnaires et de réseautage international. 
				</p> -->
				<div class="flex w-full flex-wrap gap-4">
					<button
						class="rounded-full bg-transparent px-8 py-4 font-bold uppercase tracking-widest shadow-[inset_0_0_0_2px_#616467] transition duration-200 hover:bg-[#616467] hover:text-white dark:text-neutral-200"
					>
						S'inscrire Maintenant
					</button>
					<button
						class=" rounded-full bg-transparent px-8 py-4 font-bold uppercase tracking-widest shadow-[inset_0_0_0_2px_#616467] transition duration-200 hover:bg-[#616467] hover:text-white dark:text-neutral-200 lg:hidden"
					>
						Programme
					</button>
				</div>
			</div>
			<div class="relative col-span-3 lg:col-span-2">
				<div class="relative grid grid-cols-2 gap-4">
					<div class="col-span-1 space-y-4">
						<Container>
							<div class="overflow-hidden rounded-2xl bg-gray-800">
								<img
									alt=""
									src="https://media.licdn.com/dms/image/v2/D4E22AQGPA4K6MUF7BA/feedshare-shrink_2048_1536/feedshare-shrink_2048_1536/0/1714737746033?e=1745452800&v=beta&t=CEXpok4_5up4lzlcVQAkG8I0uzGI-eBNSClnfLslSPI"
									class="h-full w-full object-cover"
								/>
							</div>
						</Container>
						<Container>
							<div class=" overflow-hidden rounded-2xl bg-gray-800">
								<img
									alt=""
									src="https://media.licdn.com/dms/image/v2/D4E22AQGd63MSiLmuSA/feedshare-shrink_2048_1536/feedshare-shrink_2048_1536/0/1715534734058?e=1745452800&v=beta&t=2XRzHF1YFomEqKCZvVu4Sl_fRWq3-hvD2tFsWbsfKi4"
									class="h-full w-full object-cover"
								/>
							</div>
						</Container>
					</div>

					<div class="col-span-1 space-y-4 pt-12">
						<Container>
							<div class=" overflow-hidden rounded-2xl bg-gray-800">
								<img
									alt=""
									src="https://media.licdn.com/dms/image/v2/D4E22AQE-pgMQlOqn8w/feedshare-shrink_2048_1536/feedshare-shrink_2048_1536/0/1715685563639?e=1745452800&v=beta&t=hX6gcJvZyw-jLYLD7TPeZcsMceU91ZStVO-gQzeC6bQ"
									class="h-full w-full object-cover"
								/>
							</div>
						</Container>
						<Container>
							<div class="overflow-hidden rounded-2xl bg-gray-800">
								<img
									alt=""
									src="https://media.licdn.com/dms/image/v2/D4E22AQFoa8GF7Tp3WA/feedshare-shrink_2048_1536/feedshare-shrink_2048_1536/0/1715685556495?e=1745452800&v=beta&t=wGPFh6dPqtrr-cXG_0_Yj6vA5eCO8R1Hy9EJAJ-Gebo"
									class="h-full w-full object-cover"
								/>
							</div>
						</Container>
					</div>
				</div>
			</div>
		</div>
	</header>
</div>
