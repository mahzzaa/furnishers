<script>
	import sofaCream from '$lib/assets/sofas/sofa-cream.jpeg';
	import sofaOrange from '$lib/assets/sofas/sofa-orange.jpeg';
	import sofaDarkBlue from '$lib/assets/sofas/sofa-dark-blue.jpeg';
	import sofaLightBlue from '$lib/assets/sofas/sofa-light-blue.jpeg';
</script>

<div
	class="relative flex items-center justify-center w-full h-full py-20 bg-surface-100 dark:bg-surface-800"
>
	<div
		class="grid items-center justify-around w-4/5 h-full grid-cols-1 2xl:grid-cols-2 xl:grid-cols-2 lg:grid-cols-2 md:grid-cols-1"
	>
		<!-- left -->
		<div
			class="flex flex-col items-center justify-center pr-5 space-y-6 2xl:items-start xl:items-start lg:items-start md:items-center"
		>
			<!-- title -->
			<div
				class="flex items-center justify-center space-x-2 text-4xl font-semibold tracking-wide text-surface-600 dark:text-surface-100"
			>
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

					<p class="px-3 py-2">About Us</p>
				</div>
			</div>
			<!-- info -->
			<div>
				<p
					class="w-full text-sm font-light text-center 2xl:w-10/12 xl:w-10/12 lg:w-10/12 md:w-full 2xl:text-justify xl:text-justify lg:text-justify md:text-center"
				>
					Lorem ipsum, dolor sit amet consectetur adipisicing elit. Illo fugiat maiores ipsa magni
					esse est dolor. Ratione velit omnis nemo repudiandae rem eius earum odit? Animi corrupti
					tempora ipsa obcaecati. <span class="text-warning-500"> see more</span>
				</p>
			</div>
		</div>
		<!-- right -->
		<div class="relative z-0 2xl:mt-20 xl:mt-20 lg:mt-20 md:mt-28 mt-28">
			<!-- upper image -->

			<div
				class="absolute z-10 w-64 -top-20 2xl:right-5 xl:right-5 lg:right-5 md:-right-10 -right-10"
			>
				<div class="relative w-64">
					<!-- squares -->
					<!-- right-top-right -->
					<div class="absolute top-0 right-0 w-2 h-2 bg-warning-500"></div>

					<!-- lines -->
					<!-- top -->
					<div class="absolute top-0.5 w-full h-[1px] bg-warning-500 opacity-70"></div>
					<!-- right -->
					<div class="absolute right-0.5 h-full w-[1px] bg-warning-500 opacity-70"></div>

					<div class="flex items-center justify-center w-64 pt-6 pr-6">
						<img src={sofaOrange} alt="sofa-orange" class="rounded-md w-fit h-fit" />
					</div>
				</div>
			</div>
			<!-- lower image -->
			<div class=" -z-0">
				<div class="relative w-[400px]">
					<!-- squares -->
					<!-- right-top-right -->
					<div class="absolute bottom-0 left-0 w-2 h-2 bg-warning-500"></div>

					<!-- lines -->
					<!-- top -->
					<div class="absolute bottom-0.5 w-full h-[1px] bg-warning-500 opacity-70"></div>
					<!-- right -->
					<div class="absolute left-0.5 h-full w-[1px] bg-warning-500 opacity-70"></div>

					<div class="flex items-center justify-center pb-6 pl-6 w-[400px]">
						<img src={sofaDarkBlue} alt="sofa-orange" class="h-64 rounded-md w-[400px]" />
					</div>
				</div>
			</div>
		</div>
	</div>
</div>
