<script>
	import ict from '$lib/assets/sponsers/ict-hub.png';
	import microsoft from '$lib/assets/sponsers/microsoft.png';
	import slack from '$lib/assets/sponsers/slack.png';
	import uberEats from '$lib/assets/sponsers/uber-eats.png';
</script>

<div
	class="flex flex-col items-center justify-around w-full py-10 space-y-8 bg-surface-200 dark:bg-surface-900"
>
	<!-- Title -->

	<div
		class="flex items-center justify-center space-x-2 text-4xl font-semibold tracking-wide text-surface-600 dark:text-surface-100"
	>
		<p>Our</p>
		<div class="relative">
			<!-- squares -->
			<!-- right-top-left -->
			<div class="absolute top-0 left-0 w-2 h-2 bg-warning-500"></div>
			<!-- right-top-right -->
			<div class="absolute top-0 right-0 w-2 h-2 bg-warning-500"></div>
			<!-- left-top-left -->
			<div class="absolute bottom-0 left-0 w-2 h-2 bg-warning-500"></div>
			<!-- left-top-right -->
			<div class="absolute bottom-0 right-0 w-2 h-2 bg-warning-500"></div>

			<!-- lines -->
			<!-- top -->
			<div class="absolute top-0.5 w-full h-[1px] bg-warning-500 opacity-70"></div>
			<!-- bottom -->
			<div class="absolute bottom-0.5 w-full h-[1px] bg-warning-500 opacity-70"></div>
			<!-- left -->
			<div class="absolute left-0.5 h-full w-[1px] bg-warning-500 opacity-70"></div>
			<!-- right -->
			<div class="absolute right-0.5 h-full w-[1px] bg-warning-500 opacity-70"></div>

			<p class="px-3 py-2">Sponser</p>
		</div>
	</div>

	<!-- Sponsers Icons -->
	<div
		class="flex items-center justify-around space-x-5 2xl:space-x-10 xl:space-x-10 lg:space-x-10 md:space-x-10 w-fit"
	>
		<!-- Uber Eats -->
		<img
			class="w-24 transition 2xl:w-32 xl:w-32 lg:w-32 md:w-32 hover:opacity-90 hover:scale-105"
			src={uberEats}
			alt="uber-eats"
		/>
		<!-- Slack -->
		<img
			class="w-24 transition 2xl:w-32 xl:w-32 lg:w-32 md:w-32 hover:opacity-90 hover:scale-105"
			src={slack}
			alt="slack"
		/>
		<!-- Microsoft -->
		<img
			class="w-24 transition 2xl:w-32 xl:w-32 lg:w-32 md:w-32 hover:opacity-90 hover:scale-105"
			src={microsoft}
			alt="microsoft"
		/>
		<!-- ICT HUB -->
		<img
			class="w-24 transition 2xl:w-32 xl:w-32 lg:w-32 md:w-32 hover:opacity-90 hover:scale-105"
			src={ict}
			alt="ict-hub"
		/>
	</div>
</div>
