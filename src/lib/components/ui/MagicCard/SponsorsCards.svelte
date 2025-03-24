<script>
	import MagicCard from './MagicCard.svelte';
</script>

<section class="mx-[10%]">
	<h1 class="my-8 text-7xl font-bold">Nos Partenaires :</h1>
	<section class=" mb-10 grid grid-cols-1 gap-10 lg:grid-cols-2">
		<div class="h-64">
			<MagicCard
				class="group h-64 cursor-pointer flex-col items-center justify-center whitespace-nowrap text-4xl shadow-2xl transition-all duration-300 hover:border-[#AF3485]"
				gradientColor="#7f486dB5"
			>
				<div
					class="flex items-center justify-center gap-1.5 font-semibold transition-all duration-500 group-hover:text-[#AF3485]"
				>
					<img class="p-32" src="/code_212.png" alt="" srcset="" />
				</div>
			</MagicCard>
		</div>
		<div class="h-64">
			<MagicCard
				class="group cursor-pointer flex-col items-center justify-center whitespace-nowrap text-4xl shadow-2xl transition-all duration-300 hover:border-[#0D4192]"
				gradientColor="#0D4192BF"
			>
				<div
					class="flex items-center justify-center gap-1.5 font-semibold transition-all duration-500 group-hover:text-[#0D4192]"
				>
					<img class="p-44" src="/ounousc.png" alt="" srcset="" />
				</div>
			</MagicCard>
		</div>
		<div class="h-64">
			<MagicCard
				class="group cursor-pointer flex-col items-center justify-center whitespace-nowrap text-4xl shadow-2xl transition-all duration-300 hover:border-white"
				gradientColor="#ffffff54"
			>
				<div
					class="flex items-center justify-center gap-1.5 font-semibold transition-all duration-500 group-hover:text-white"
				>
					<img class="w-44" src="/oja_logo.png" alt="" srcset="" />
				</div>
			</MagicCard>
		</div>
		<div class="h-64">
			<MagicCard
				class="group cursor-pointer flex-col items-center justify-center whitespace-nowrap text-4xl shadow-2xl transition-all duration-300 hover:border-[#098B36]"
				gradientColor="#098B3654"
			>
				<div
					class="flex items-center justify-center gap-1.5 font-semibold transition-all duration-500 group-hover:text-[#0D4192]"
				>
					<img class="p-44" src="/emsi_logo.png" alt="" srcset="" />
				</div>
			</MagicCard>
		</div>
	</section>
</section>
