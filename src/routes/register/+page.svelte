<script lang="ts">
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
	<div class="grid grid-cols-1 gap-6 md:grid-cols-2 lg:grid-cols-3">
		<!-- Workshop Card 1 -->
		<div class="rounded-xl border border-slate-800 p-6 transition-colors hover:border-slate-700">
			<div class="mb-4 flex items-start justify-between">
				<span class="rounded-full bg-blue-500/20 px-3 py-1 text-sm text-blue-400">Beginner</span>
				<span class="text-sm text-slate-500">Free</span>
			</div>

			<h3 class="mb-2 text-xl font-semibold text-slate-100">Intro to React</h3>

			<div class="mb-4 flex items-center gap-2 text-slate-400">
				<i data-lucide="calendar-days" class="h-4 w-4"></i>
				<span class="text-sm">Sept 25, 2023</span>
			</div>

			<p class="mb-6 line-clamp-3 text-sm text-slate-400">
				Learn the fundamentals of React including components, props, and state management. Perfect
				for developers new to frontend frameworks.
			</p>

			<a
				href="#"
				class="inline-flex w-full items-center justify-between rounded-lg bg-slate-800 px-4 py-2 transition-colors hover:bg-slate-700"
			>
				<span class="text-sm text-slate-300">Register Now</span>
				<i data-lucide="arrow-up-right" class="h-4 w-4 text-blue-500"></i>
			</a>
		</div>

		<!-- Workshop Card 2 -->
		<div class="rounded-xl border border-slate-800 p-6 transition-colors hover:border-slate-700">
			<div class="mb-4 flex items-start justify-between">
				<span class="rounded-full bg-purple-500/20 px-3 py-1 text-sm text-purple-400">Advanced</span
				>
				<span class="text-sm text-slate-500">$49.99</span>
			</div>

			<h3 class="mb-2 text-xl font-semibold text-slate-100">State Management with Redux</h3>

			<div class="mb-4 flex items-center gap-2 text-slate-400">
				<i data-lucide="calendar-days" class="h-4 w-4"></i>
				<span class="text-sm">Oct 2, 2023</span>
			</div>

			<p class="mb-6 line-clamp-3 text-sm text-slate-400">
				Master complex state management patterns using Redux Toolkit. Learn best practices for
				large-scale applications.
			</p>

			<a
				href="#"
				class="inline-flex w-full items-center justify-between rounded-lg bg-slate-800 px-4 py-2 transition-colors hover:bg-slate-700"
			>
				<span class="text-sm text-slate-300">Register Now</span>
				<i data-lucide="arrow-up-right" class="h-4 w-4 text-blue-500"></i>
			</a>
		</div>

		<!-- Workshop Card 3 -->
		<div class="rounded-xl border border-slate-800 p-6 transition-colors hover:border-slate-700">
			<div class="mb-4 flex items-start justify-between">
				<span class="rounded-full bg-emerald-500/20 px-3 py-1 text-sm text-emerald-400"
					>Intermediate</span
				>
				<span class="text-sm text-slate-500">$29.99</span>
			</div>

			<h3 class="mb-2 text-xl font-semibold text-slate-100">Next.js Fundamentals</h3>

			<div class="mb-4 flex items-center gap-2 text-slate-400">
				<i data-lucide="calendar-days" class="h-4 w-4"></i>
				<span class="text-sm">Oct 9, 2023</span>
			</div>

			<p class="mb-6 line-clamp-3 text-sm text-slate-400">
				Build full-stack applications with Next.js. Covers routing, API routes, and static site
				generation.
			</p>

			<a
				href="#"
				class="inline-flex w-full items-center justify-between rounded-lg bg-slate-800 px-4 py-2 transition-colors hover:bg-slate-700"
			>
				<span class="text-sm text-slate-300">Register Now</span>
				<i data-lucide="arrow-up-right" class="h-4 w-4 text-blue-500"></i>
			</a>
		</div>
	</div>
</div>

<div class="h-44"></div>
