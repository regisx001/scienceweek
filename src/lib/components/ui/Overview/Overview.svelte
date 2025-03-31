<script>
	import { SimpleCard2, SimpleCard3 } from '../cards/index.js';
</script>

<div class="mx-[10%] mt-10 bg-background p-8 shadow-sm">
	<!-- Title -->
	<h2 class="mb-12 text-center text-4xl font-bold text-foreground">Science Week en Bref</h2>

	<!-- Three Column Layout -->
	<div class=" grid gap-8 md:grid-cols-3">
		<!-- Conferences -->

		<SimpleCard2>
			<div class="space-y-4 p-6 transition-all hover:shadow-md">
				<div class="flex items-center gap-3">
					<div class="rounded-full bg-primary/10 p-3">
						<svg class="h-6 w-6 text-primary" fill="none" stroke="currentColor" viewBox="0 0 24 24">
							<path
								stroke-linecap="round"
								stroke-linejoin="round"
								stroke-width="2"
								d="M8 7V3m8 4V3m-9 8h10M5 21h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v12a2 2 0 002 2z"
							/>
						</svg>
					</div>
					<h3 class="text-lg font-semibold text-foreground">Conférences</h3>
				</div>
				<p class="text-sm text-muted-foreground">
					Lors de Science Week, des conférences captivantes ont exploré l'astronomie, la biologie,
					la chimie, l'ingénierie industrielle, la physique, les mathématiques et l'informatique,
					offrant aux participants un aperçu des avancées et défis scientifiques actuels.
				</p>
				<div class="pt-2">
					<span
						class="inline-block rounded-full bg-primary/10 px-3 py-1 text-xs font-medium text-primary"
					>
						7 disciplines couvertes
					</span>
				</div>
			</div>
		</SimpleCard2>
		<SimpleCard3>
			<!-- Workshops -->
			<div class="space-y-4 p-6 transition-all hover:shadow-md">
				<div class="flex items-center gap-3">
					<div class="rounded-full bg-primary/10 p-3">
						<svg class="h-6 w-6 text-primary" fill="none" stroke="currentColor" viewBox="0 0 24 24">
							<path
								stroke-linecap="round"
								stroke-linejoin="round"
								stroke-width="2"
								d="M19.428 15.428a2 2 0 00-1.022-.547l-2.387-.477a6 6 0 00-3.86.517l-.318.158a6 6 0 01-3.86.517L6.05 15.21a2 2 0 00-1.806.547M8 4h8l-1 1v5.172a2 2 0 00.586 1.414l5 5c1.26 1.26.367 3.414-1.415 3.414H4.828c-1.782 0-2.674-2.154-1.414-3.414l5-5A2 2 0 009 10.172V5L8 4z"
							/>
						</svg>
					</div>
					<h3 class="text-lg font-semibold text-foreground">Ateliers</h3>
				</div>
				<p class="text-sm text-muted-foreground">
					Les ateliers de Science Week ont offert aux participants une approche interactive des
					sciences, avec des expériences pratiques en astronomie, biologie, chimie, ingénierie
					industrielle, physique et informatique.
				</p>
				<div class="pt-2">
					<span
						class="inline-block rounded-full bg-primary/10 px-3 py-1 text-xs font-medium text-primary"
					>
						6 domaines pratiques
					</span>
				</div>
			</div>
		</SimpleCard3>
		<SimpleCard2>
			<!-- First Edition -->
			<div class="space-y-4 p-6 transition-all hover:shadow-md">
				<div class="flex items-center gap-3">
					<div class="rounded-full bg-primary/10 p-3">
						<svg class="h-6 w-6 text-primary" fill="none" stroke="currentColor" viewBox="0 0 24 24">
							<path
								stroke-linecap="round"
								stroke-linejoin="round"
								stroke-width="2"
								d="M9 12l2 2 4-4m5.618-4.016A11.955 11.955 0 0112 2.944a11.955 11.955 0 01-8.618 3.04A12.02 12.02 0 003 9c0 5.591 3.824 10.29 9 11.622 5.176-1.332 9-6.03 9-11.622 0-1.042-.133-2.052-.382-3.016z"
							/>
						</svg>
					</div>
					<h3 class="text-lg font-semibold text-foreground">1ère Édition</h3>
				</div>
				<p class="text-sm text-muted-foreground">
					Science Week 1 a attiré plus de 400 participants par jour pour les conférences, ateliers
					et visites, illustrant l'intérêt croissant pour l'exploration des sciences et le partage
					des connaissances.
				</p>
				<div class="pt-2">
					<span
						class="inline-block rounded-full bg-primary/10 px-3 py-1 text-xs font-medium text-primary"
					>
						400+ participants/jour
					</span>
				</div>
			</div>
		</SimpleCard2>
	</div>
</div>
