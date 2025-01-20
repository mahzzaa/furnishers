<script>
	// /** @satisfies {import('./$types').Actions} */
	export const actions = {
		default: async (event) => {
			// TODO log the user in
		}
	};
</script>

<div
	class="relative flex flex-col items-center justify-center w-full h-full py-20 space-y-7 bg-surface-100 dark:bg-surface-800"
>
	<!-- Title -->
	<div
		class="flex items-center justify-center space-x-2 text-4xl font-semibold tracking-wide text-surface-600 dark:text-surface-100"
	>
		<p>Join</p>
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

			<p class="px-3 py-2">With Us</p>
		</div>
	</div>

	<!-- info -->
	<div class="w-4/5 2xl:w-full xl:w-full lg:w-full md:w-full">
		<p class="text-sm font-light text-center">
			Lorem ipsum dolor sit amet consectetur adipisicing elit. Nam nemo a quos sit recusandae
			consequuntur.
		</p>
	</div>

	<!-- content + form -->
	<div
		class="grid items-center justify-center w-4/5 grid-cols-1 2xl:w-w-4/5 xl:w-w-4/5 lg:w-w-4/5 md:w-4/5 2xl:grid-cols-2 xl:grid-cols-2 lg:grid-cols-2 md:grid-cols-1 2xl:gap-x-10 xl:gap-x-10 lg:gap-x-10 md:gap-x-0 gap-x-0 2xl:gap-y-0 xl:gap-y-0 lg:gap-y-0 md:gap-y-10 gap-y-10"
	>
		<!-- video  -->
		<div class="flex items-center justify-start">
			<iframe
				class="w-full rounded-md h-72"
				src="https://www.youtube.com/embed/8Lmp1Ncaa7Y?si=QBVLAmaYtWo8lXGX"
				title="YouTube video player"
				frameborder="0"
				allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
				referrerpolicy="strict-origin-when-cross-origin"
				allowfullscreen
			></iframe>
		</div>

		<!-- form -->
		<form method="POST" class="flex flex-col w-full space-y-5">
			<label>
				<input
					class="w-full h-12 border-0 rounded-md dark:placeholder:text-surface-100/50 placeholder:text-surface-900/50 variant-glass-surface"
					placeholder="Email"
					name="email"
					type="email"
				/>
			</label>
			<label>
				<input
					class="w-full h-12 border-0 rounded-md dark:placeholder:text-surface-100/50 placeholder:text-surface-900/50 variant-glass-surface"
					placeholder="Password"
					name="password"
					type="password"
				/>
			</label>
			<div
				class="flex items-center justify-center w-full 2xl:justify-start xl:justify-start lg:justify-start md:justify-center"
			>
				<button
					class="px-16 py-3 text-sm font-semibold border-2 border-transparent rounded-md text-surface-100 bg-surface-600 hover:bg-white hover:border-2 hover:border-surface-600 hover:text-surface-600"
				>
					Sign up
				</button>
			</div>
		</form>
	</div>
</div>
