<script lang="ts">
	let workshopData: WorkshopProps = $props();
</script>

<div class="z-50 border border-slate-800 p-6 transition-colors hover:border-slate-700">
	<h3 class="mb-2 text-xl font-semibold text-slate-100">{workshopData.title}</h3>

	<div class="mb-4 flex items-center gap-2 text-slate-400">
		<i data-lucide="calendar-days" class="h-4 w-4"></i>
		<span class="text-sm">{workshopData.date}</span>
	</div>

	<p class="mb-6 line-clamp-5 text-sm text-slate-400">
		{workshopData.description}
	</p>

	<a
		href={workshopData.link}
		target="_blank"
		class=" flex w-full items-center justify-center rounded-lg bg-slate-800 px-4 py-2 transition-colors hover:bg-slate-700"
	>
		<span class="text-lg font-bold text-slate-300">S'inscrire Maintenant</span>
	</a>
</div>
