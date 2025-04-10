<script>
	import { base } from '$app/paths';
</script>

<footer class="border-t bg-background/95">
	<div class="px-4 py-12 sm:py-16 lg:mx-[10%]">
		<div class="grid grid-cols-1 gap-8 sm:grid-cols-2 md:grid-cols-3 lg:grid-cols-4">
			<!-- Event Info -->
			<div class="space-y-4">
				<div class="flex items-center gap-2">
					<svg
						class="h-6 w-6 shrink-0 text-primary"
						fill="none"
						stroke="currentColor"
						viewBox="0 0 24 24"
					>
						<path
							stroke-linecap="round"
							stroke-linejoin="round"
							stroke-width="2"
							d="M19 14l-7 7m0 0l-7-7m7 7V3"
						/>
					</svg>
					<span class="text-lg font-semibold">ScienceWeek 2025</span>
				</div>
				<p class="text-sm text-muted-foreground">
					Promoting scientific innovation through collaboration and education
				</p>
			</div>

			<!-- Quick Links -->
			<div class="space-y-3">
				<h3 class="text-sm font-medium">Navigation</h3>
				<nav class="space-y-2">
					<a
						href="{base}/"
						class="block py-1 text-sm text-muted-foreground transition-colors hover:text-foreground"
					>
						Home
					</a>
					<a
						href="{base}/register"
						class="block py-1 text-sm text-muted-foreground transition-colors hover:text-foreground"
					>
						Inscription
					</a>
					<a
						href="{base}/program"
						class="block py-1 text-sm text-muted-foreground transition-colors hover:text-foreground"
					>
						Programme
					</a>
				</nav>
			</div>

			<!-- Contact -->
			<div class="space-y-3">
				<h3 class="text-sm font-medium">Contact</h3>
				<div class="space-y-2 text-sm text-muted-foreground">
					<div class="flex items-start gap-2">
						<svg
							class="mt-0.5 h-4 w-4 shrink-0"
							fill="none"
							stroke="currentColor"
							viewBox="0 0 24 24"
						>
							<path
								stroke-linecap="round"
								stroke-linejoin="round"
								stroke-width="2"
								d="M3 8l7.89 5.26a2 2 0 002.22 0L21 8M5 19h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z"
							/>
						</svg>
						<a href="mailto:contact@scienceweek.fr" class="transition-colors hover:text-foreground">
							lgdfsttclub@gmail.com
						</a>
					</div>
					<div class="flex items-start gap-2">
						<svg
							class="mt-0.5 h-4 w-4 shrink-0"
							fill="none"
							stroke="currentColor"
							viewBox="0 0 24 24"
						>
							<path
								stroke-linecap="round"
								stroke-linejoin="round"
								stroke-width="2"
								d="M3 5a2 2 0 012-2h3.28a1 1 0 01.948.684l1.498 4.493a1 1 0 01-.502 1.21l-2.257 1.13a11.042 11.042 0 005.516 5.516l1.13-2.257a1 1 0 011.21-.502l4.493 1.498a1 1 0 01.684.949V19a2 2 0 01-2 2h-1C9.716 21 3 14.284 3 6V5z"
							/>
						</svg>
						<a href="tel:+33123456789" class="transition-colors hover:text-foreground">
							+212 622-188776
						</a>
					</div>
				</div>
			</div>

			<!-- Social -->
			<div class="space-y-3">
				<h3 class="text-sm font-medium">Connect</h3>
				<div class="flex gap-4">
					<a
						aria-label="Instagram"
						href="https://www.instagram.com/thelgdclub.fstt/"
						target="_blank"
						class="-m-2 p-2 text-muted-foreground transition-colors hover:text-foreground"
					>
						<svg
							xmlns="http://www.w3.org/2000/svg"
							width="24"
							height="24"
							viewBox="0 0 24 24"
							fill="none"
							stroke="currentColor"
							stroke-width="2"
							stroke-linecap="round"
							stroke-linejoin="round"
							class="icon icon-tabler icons-tabler-outline icon-tabler-brand-instagram"
							><path stroke="none" d="M0 0h24v24H0z" fill="none" /><path
								d="M4 8a4 4 0 0 1 4 -4h8a4 4 0 0 1 4 4v8a4 4 0 0 1 -4 4h-8a4 4 0 0 1 -4 -4z"
							/><path d="M9 12a3 3 0 1 0 6 0a3 3 0 0 0 -6 0" /><path d="M16.5 7.5v.01" /></svg
						>
						<!-- Add other social icons -->
					</a>

					<a
						aria-label="Instagram"
						href="https://www.tiktok.com/@thelgdclub.fstt"
						target="_blank"
						class="-m-2 p-2 text-muted-foreground transition-colors hover:text-foreground"
					>
						<svg
							xmlns="http://www.w3.org/2000/svg"
							width="24"
							height="24"
							viewBox="0 0 24 24"
							fill="none"
							stroke="currentColor"
							stroke-width="2"
							stroke-linecap="round"
							stroke-linejoin="round"
							class="icon icon-tabler icons-tabler-outline icon-tabler-brand-tiktok"
							><path stroke="none" d="M0 0h24v24H0z" fill="none" /><path
								d="M21 7.917v4.034a9.948 9.948 0 0 1 -5 -1.951v4.5a6.5 6.5 0 1 1 -8 -6.326v4.326a2.5 2.5 0 1 0 4 2v-11.5h4.083a6.005 6.005 0 0 0 4.917 4.917z"
							/></svg
						>
						<!-- Add other social icons -->
					</a>
					<a
						aria-label="Instagram"
						href="https://www.linkedin.com/in/legends-fstt-club-0723a4336/?original_referer=https%3A%2F%2Fwww%2Egoogle%2Ecom%2F&originalSubdomain=ma"
						target="_blank"
						class="-m-2 p-2 text-muted-foreground transition-colors hover:text-foreground"
					>
						<svg
							xmlns="http://www.w3.org/2000/svg"
							width="24"
							height="24"
							viewBox="0 0 24 24"
							fill="none"
							stroke="currentColor"
							stroke-width="2"
							stroke-linecap="round"
							stroke-linejoin="round"
							class="icon icon-tabler icons-tabler-outline icon-tabler-brand-linkedin"
							><path stroke="none" d="M0 0h24v24H0z" fill="none" /><path d="M8 11v5" /><path
								d="M8 8v.01"
							/><path d="M12 16v-5" /><path d="M16 16v-3a2 2 0 1 0 -4 0" /><path
								d="M3 7a4 4 0 0 1 4 -4h10a4 4 0 0 1 4 4v10a4 4 0 0 1 -4 4h-10a4 4 0 0 1 -4 -4z"
							/></svg
						>
						<!-- Add other social icons -->
					</a>

					<a
						aria-label="Instagram"
						href="https://github.com/regisx001/scienceweek"
						target="_blank"
						class="-m-2 p-2 text-muted-foreground transition-colors hover:text-foreground"
					>
						<svg
							xmlns="http://www.w3.org/2000/svg"
							width="24"
							height="24"
							viewBox="0 0 24 24"
							fill="none"
							stroke="currentColor"
							stroke-width="2"
							stroke-linecap="round"
							stroke-linejoin="round"
							class="icon icon-tabler icons-tabler-outline icon-tabler-brand-github"
							><path stroke="none" d="M0 0h24v24H0z" fill="none" /><path
								d="M9 19c-4.3 1.4 -4.3 -2.5 -6 -3m12 5v-3.5c0 -1 .1 -1.4 -.5 -2c2.8 -.3 5.5 -1.4 5.5 -6a4.6 4.6 0 0 0 -1.3 -3.2a4.2 4.2 0 0 0 -.1 -3.2s-1.1 -.3 -3.5 1.3a12.3 12.3 0 0 0 -6.2 0c-2.4 -1.6 -3.5 -1.3 -3.5 -1.3a4.2 4.2 0 0 0 -.1 3.2a4.6 4.6 0 0 0 -1.3 3.2c0 4.6 2.7 5.7 5.5 6c-.6 .6 -.6 1.2 -.5 2v3.5"
							/></svg
						>
						<!-- Add other social icons -->
					</a>
				</div>
			</div>
		</div>

		<!-- Copyright -->
		<div class="mt-12 border-t pt-8">
			<div class="flex flex-col items-center gap-4 text-center sm:flex-row sm:justify-between">
				<p class="text-sm text-muted-foreground">© 2025 Science Week. All rights reserved.</p>
				<div class="flex flex-wrap justify-center gap-4">
					<a
						href="##"
						class="text-sm text-muted-foreground transition-colors hover:text-foreground"
					>
						Developed By : Ezzoubair Zarqi
					</a>
					<a
						target="_blank"
						href="https://github.com/regisx001/scienceweek"
						class="text-sm text-muted-foreground transition-colors hover:text-foreground"
					>
						Github
					</a>
				</div>
			</div>
		</div>
	</div>
</footer>
