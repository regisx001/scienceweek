<script>
	import { base } from '$app/paths';
	import MagicCard from './MagicCard.svelte';
</script>

<section class="mx-[10%]">
	<h1 class="mb-16 text-4xl font-bold">Nos Partenaires :</h1>
	<section class=" mb-10 grid grid-rows-1 gap-10 lg:grid-cols-3">
		<div class="h-32 lg:h-48">
			<MagicCard
				class="group cursor-pointer flex-col items-center justify-center whitespace-nowrap text-4xl shadow-2xl transition-all duration-300 hover:border-[#AF3485]"
				gradientColor="#7f486dB5"
			>
				<div
					class="flex items-center justify-center gap-1.5 font-semibold transition-all duration-500 group-hover:text-[#AF3485]"
				>
					<img class="w-48 lg:w-80" src="{base}/code_212.png" alt="" srcset="" />
				</div>
			</MagicCard>
		</div>
		<div class="h-32 lg:h-48">
			<MagicCard
				class="group cursor-pointer flex-col items-center justify-center whitespace-nowrap text-4xl shadow-2xl transition-all duration-300 hover:border-[#0D4192]"
				gradientColor="#0D4192BF"
			>
				<div
					class="flex items-center justify-center gap-1.5 font-semibold transition-all duration-500 group-hover:text-[#0D4192]"
				>
					<img class="w-36 lg:w-44" src="{base}/ounousc.png" alt="" srcset="" />
				</div>
			</MagicCard>
		</div>
		<div class="h-32 lg:h-48">
			<MagicCard
				class="group cursor-pointer flex-col items-center justify-center whitespace-nowrap text-4xl shadow-2xl transition-all duration-300 hover:border-white"
				gradientColor="#ffffff54"
			>
				<div
					class="flex items-center justify-center gap-1.5 font-semibold transition-all duration-500 group-hover:text-white"
				>
					<img class="w-28 lg:w-44" src="{base}/oja_logo.png" alt="" srcset="" />
				</div>
			</MagicCard>
		</div>
		<div class="h-32 lg:h-48">
			<MagicCard
				class="group cursor-pointer flex-col items-center justify-center whitespace-nowrap text-4xl shadow-2xl transition-all duration-300 hover:border-[#098B36]"
				gradientColor="#098B3654"
			>
				<div
					class="flex items-center justify-center gap-1.5 font-semibold transition-all duration-500 group-hover:text-[#0D4192]"
				>
					<img class="w-48 lg:w-80" src="{base}/emsi_logo.png" alt="" srcset="" />
				</div>
			</MagicCard>
		</div>

		<div class="h-32 lg:h-48">
			<MagicCard
				class="group cursor-pointer flex-col items-center justify-center whitespace-nowrap text-4xl shadow-2xl transition-all duration-300 hover:border-[#F4C90054]"
				gradientColor="#F4C90054"
			>
				<div
					class="flex items-center justify-center gap-1.5 font-semibold transition-all duration-500 group-hover:text-[#0D4192]"
				>
					<img class="w-28 lg:w-44" src="{base}/fstt_logo.png" alt="" srcset="" />
				</div>
			</MagicCard>
		</div>
	</section>
</section>
