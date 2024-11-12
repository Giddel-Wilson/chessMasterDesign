<script>
	const navigationLinks = ['ABOUT', 'GAMES', 'BLOG', 'CONTACT'];
	import { Button } from '$lib/components/ui/button';
	import chessPiece from '$lib/assets/chessPiece.png';
	import chessPiece2 from '$lib/assets/chessPiece2.png';
	import me from '$lib/assets/profile.png';
</script>

<div class="max-w-screen min-h-screen bg-white text-black lg:overflow-hidden">
	<!-- Header -->
	<header class="flex flex-col border-b border-black sm:flex-row">
		<div class="flex-1 border-black p-4 sm:border-r">
			<div class="flex items-center gap-4">
				<div class="h-8 w-8 bg-black"></div>
				<h1 class="font-serif text-3xl italic sm:text-4xl">Giddel Wilson</h1>
			</div>
		</div>
		<div
			class="w-full border-e border-t border-e-black border-t-black p-4 text-sm sm:w-32 sm:border-l sm:border-t-0"
		>
			<div class="flex justify-between">
				<span>Pg.</span>
				<span>01</span>
				<span>Ru</span>
			</div>
			<div class="mt-4 text-right">MENU</div>
		</div>
	</header>

	<!-- Hero Section -->
	<div class="flex flex-col border-b border-black sm:flex-row">
		<div
			class="w-full border-b border-black p-4 font-serif text-2xl italic sm:w-32 sm:border-b-0 sm:border-r"
		>
			Grand
		</div>
		<div class="relative min-h-[300px] flex-1 sm:min-h-[400px]">
			<div class="pointer-events-none absolute inset-0 grid grid-cols-3 sm:grid-cols-6">
				{#each Array(6) as _, i}
					<div class="border-r border-black"></div>
				{/each}
			</div>
			<div class="pointer-events-none absolute inset-0 grid grid-rows-4">
				{#each Array(4) as _, i}
					<div class="border-b border-black"></div>
				{/each}
			</div>
			<img
				src={chessPiece2}
				alt="Chess Piece"
				class="right-1/5 absolute top-1/2 w-96 -translate-y-1/2 sm:w-64 md:left-1/4 md:w-[80vw] lg:left-2/4 lg:w-[700px]"
			/>
			<h2
				class="absolute right-4 top-1/2 -translate-y-1/2 font-serif text-4xl sm:right-32 sm:text-6xl"
			>
				GIDDEL
			</h2>
		</div>
		<div
			class="w-full border-t border-black p-4 font-serif text-2xl italic sm:w-32 sm:rotate-180 sm:border-l sm:border-t-0 sm:[writing-mode:vertical-lr]"
		>
			WILSON
		</div>
	</div>

	<!-- About Section -->
	<section class="flex flex-col border-b border-black sm:flex-row">
		<div class="w-full border-b border-black p-4 sm:w-32 sm:border-b-0 sm:border-r">
			<span class="text-sm">01.</span>
			<h3 class="mt-2 font-serif text-2xl italic">About</h3>
		</div>
		<div class="relative min-h-[600px] flex-1 sm:min-h-[400px]">
			<div class="pointer-events-none absolute inset-0 grid grid-cols-3 sm:grid-cols-6">
				{#each Array(6) as _, i}
					<div class="border-r border-black"></div>
				{/each}
			</div>
			<div class="pointer-events-none absolute inset-0 grid grid-rows-4">
				{#each Array(4) as _, i}
					<div class="border-b border-black"></div>
				{/each}
			</div>

			<div class="absolute z-20 max-w-xl p-4 sm:p-8 md:p-0 lg:p-4">
				<p
					class="mb-8 w-full border border-black bg-transparent p-4 md:w-[48vw] md:bg-white lg:w-full"
				>
					Giddel Wilson is a Frontend software engineer specializing in Sveltekit and Tailwind CSS. Passionate about
					building responsive, user-friendly web interfaces while expanding his expertise in modern
					web practices; with interest in other fields such as Cybersecurity & AI/ML. 
				</p>
				<Button
					variant="outline"
					class="absolute rounded-none border-black bg-white hover:bg-black hover:text-white"
					>LEARN MORE</Button
				>
			</div>

			<div class="absolute right-0 top-0 w-full border border-black bg-white p-4 sm:w-64">
				<img
					src="https://i.pinimg.com/236x/90/04/22/900422ab7d276bcce192b2ff09587f90.jpg"
					alt="Chess Piece"
					class="w-full border-b border-b-black opacity-50 md:opacity-100"
				/>
				<div class="border-black pt-4 text-center">
					<div class="mb-2 font-serif italic">Grand master</div>
					<div class="mb-1 text-4xl">2773</div>
					<div class="text-sm">March 2023</div>
				</div>
			</div>

			<div
				class="absolute bottom-0 left-0 flex w-full border-b border-e border-b-black border-e-black bg-white sm:w-64"
			>
				<div class="flex-1 border-r border-t border-black p-4 text-center">
					<div class="mb-2 text-sm">CONTRIBUTION</div>
					<div class="mb-1 text-4xl">235</div>
					<div class="text-sm">Nov 2024</div> 
				</div>
				<div class="flex-1 border-t border-black p-4 text-center">
					<div class="mb-2 text-sm">REPOS</div>
					<div class="mb-1 text-4xl">No.0</div>
					<div class="text-sm">2024</div>
				</div>
			</div>
		</div>
	</section>

	<!-- Games Section -->
	<section class="flex flex-col border-b border-black sm:flex-row">
		<div class="w-full border-b border-black p-4 sm:w-32 sm:border-b-0 sm:border-r">
			<span class="text-sm">02.</span>
			<h3 class="mt-2 font-serif text-2xl italic">Games</h3>
		</div>
		<div class="relative min-h-[600px] flex-1 sm:min-h-[400px]">
			<div class="pointer-events-none absolute inset-0 grid grid-cols-3 sm:grid-cols-6">
				{#each Array(6) as _, i}
					<div class="border-r border-black"></div>
				{/each}
			</div>
			<div class="pointer-events-none absolute inset-0 grid grid-rows-4">
				{#each Array(4) as _, i}
					<div class="border-b border-black"></div>
				{/each}
			</div>

			<div class="absolute bg-white p-4 sm:p-8 md:bg-transparent">
				<p class="mb-8 bg-white">Live games and selection of the games played by Levon</p>
				<Button variant="outline" class="rounded-none border-black hover:bg-black hover:text-white"
					>LEARN MORE</Button
				>
			</div>

			<div class="absolute bottom-0 right-4 me-32 w-64 sm:right-32 sm:w-96">
				<img src={chessPiece2} alt="Chess Piece" class="w-full" />
			</div>

			<div class="absolute bottom-4 right-0 flex p-4 md:top-10 md:flex-col lg:top-8">
				<h4 class="mb-8 ms-auto w-max font-serif text-2xl italic md:bg-white md:text-right">
					Medal Record
				</h4>
				<div class="grid grid-cols-2 gap-4">
					{#each [{ year: 2006, type: 'GOLD' }, { year: 2006, type: 'GOLD' }, { year: 2012, type: 'GOLD' }, { year: 2008, type: 'BRONZE' }] as medal}
						<div
							class="flex h-24 w-24 flex-col items-center justify-center rounded-full border border-black sm:h-32 sm:w-32"
						>
							<div class="text-3xl sm:text-4xl">1</div>
							<div class="text-sm font-bold sm:text-base">{medal.type}</div>
							<div class="text-xs sm:text-sm">Turin {medal.year}</div>
						</div>
					{/each}
				</div>
			</div>
		</div>
	</section>

	<!-- Footer -->
	<footer class="border-t border-black text-sm">
		<!-- Top Row -->
		<div class="flex justify-between border-b border-black px-8 py-4">
			<div class="flex flex-wrap gap-8">
				<a href="/" class="hover:underline">FACEBOOK</a>
				<a href="/" class="hover:underline">INSTAGRAM</a>
				<a href="/" class="hover:underline">TWITTER</a>
				<a href="/" class="hover:underline">YOUTUBE</a>
				<a href="mailto:info@giddelwilson.com" class="hover:underline"> info@giddelwilson.com </a>
			</div>
		</div>

		<!-- Bottom Row -->
		<div class="flex flex-col md:flex-row">
			<!-- Copyright Section -->
			<div class="w-full border-b border-r border-black p-4 md:w-[240px]">
				<div>2024</div>
				<div>ALL RIGHT RESERVED</div>
				<div>
					MADE BY <span class="border-b border-black">GIDDEL WILSON</span>
				</div>
			</div>
			<!-- Logo Circle -->
			<div
				class="relative hidden w-[120px] items-center justify-center border-r border-black md:flex"
			>
				<div class="h-16 w-16 rounded-full border-2 border-black"></div>
			</div>

			<!-- Navigation Links -->
			<div class="flex flex-1 p-5 md:p-0">
				{#each navigationLinks as item}
					<a
						href="/"
						class="flex flex-1 items-center justify-center border-r border-black transition-colors last:border-r-0 hover:bg-black hover:text-white"
					>
						{item}
					</a>
				{/each}
			</div>
		</div>
	</footer>
</div>

<style>
	:global(body) {
		margin: 0;
		padding: 0;
	}
</style>
