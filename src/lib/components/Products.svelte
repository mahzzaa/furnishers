<script>
	import { Ratings } from '@skeletonlabs/skeleton';
	import furniture from '../assets/furniture.jpeg';
	import sofaBlue from '../assets/sofas/sofa-dark-blue.jpeg';
	let products = [
		{
			image: furniture,
			name: 'Product 1',
			stars: 4,
			price: 100,
			info: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Nam nemo a quos sit recusandae consequuntur.',
			link: 'https://www.google.com'
		},
		{
			image: sofaBlue,
			name: 'Product 2',
			stars: 3,
			price: 200,
			info: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Nam nemo a quos sit recusandae consequuntur.',
			link: 'https://www.google.com'
		}
	];
</script>

<div
	class="relative flex flex-col items-center justify-center w-full h-full py-20 bg-surface-100 dark:bg-surface-800"
>
	<!-- title + info -->
	<div class="flex flex-col items-center justify-center space-y-5">
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

				<p class="px-3 py-2">Products</p>
			</div>
		</div>
		<!-- info -->
		<p class="w-4/5 px-5 text-sm font-light text-center 2xl:w-full xl:w-full lg:w-full md:w-full">
			Nam nemo a quos sit recusandae consequuntur.Lorem ipsum dolor sit amet consectetur adipisicing
			elit.
		</p>
	</div>

	<!-- cards -->

	<div class="relative flex items-center justify-around mt-10">
		<div
			class="relative grid w-4/5 grid-cols-1 2xl:grid-cols-2 xl:grid-cols-2 lg:grid-cols-2 md:grid-cols-2"
		>
			<!-- decoration -->
			<div class="absolute top-0 left-0 w-2 h-2 bg-warning-500"></div>
			<div class="absolute top-0 right-0 w-2 h-2 bg-warning-500"></div>

			<div class="absolute top-0.5 left-0 w-10 h-[1px] bg-warning-500 opacity-70"></div>
			<div class="absolute top-0.5 right-0 w-10 h-[1px] bg-warning-500 opacity-70"></div>
			<div class="absolute top-0.5 right-0.5 w-[1px] h-10 bg-warning-500 opacity-70"></div>
			<div class="absolute top-0.5 left-0.5 w-[1px] h-10 bg-warning-500 opacity-70"></div>

			<!-- card -->
			{#each products as product}
				<div class="m-5 space-y-5">
					<!-- image -->
					<div>
						<img class="w-full h-full rounded-md" src={product.image} alt={product.name} />
					</div>

					<!-- product's name + stars -->
					<div class="space-y-2">
						<!-- product's name + stars -->
						<div class="flex items-center justify-between">
							<!-- name -->
							<p class="text-xl font-semibold">
								{product.name}
							</p>
							<!-- stars -->
							<div>
								<Ratings value={product.stars} max={5}>
									<svelte:fragment slot="empty">
										<svg
											viewBox="0 0 128 128"
											xmlns="http://www.w3.org/2000/svg"
											xmlns:xlink="http://www.w3.org/1999/xlink"
											aria-hidden="true"
											role="img"
											class="w-4 h-4 iconify iconify--noto"
											preserveAspectRatio="xMidYMid meet"
											fill="#000000"
											><g id="SVGRepo_bgCarrier" stroke-width="0"></g><g
												id="SVGRepo_tracerCarrier"
												stroke-linecap="round"
												stroke-linejoin="round"
											></g><g id="SVGRepo_iconCarrier"
												><path
													d="M68.05 7.23l13.46 30.7a7.047 7.047 0 0 0 5.82 4.19l32.79 2.94c3.71.54 5.19 5.09 2.5 7.71l-24.7 20.75c-2 1.68-2.91 4.32-2.36 6.87l7.18 33.61c.63 3.69-3.24 6.51-6.56 4.76L67.56 102a7.033 7.033 0 0 0-7.12 0l-28.62 16.75c-3.31 1.74-7.19-1.07-6.56-4.76l7.18-33.61c.54-2.55-.36-5.19-2.36-6.87L5.37 52.78c-2.68-2.61-1.2-7.17 2.5-7.71l32.79-2.94a7.047 7.047 0 0 0 5.82-4.19l13.46-30.7c1.67-3.36 6.45-3.36 8.11-.01z"
													fill="#fdd835"
												></path><path
													d="M67.07 39.77l-2.28-22.62c-.09-1.26-.35-3.42 1.67-3.42c1.6 0 2.47 3.33 2.47 3.33l6.84 18.16c2.58 6.91 1.52 9.28-.97 10.68c-2.86 1.6-7.08.35-7.73-6.13z"
													fill="#ffff8d"
												></path><path
													d="M95.28 71.51L114.9 56.2c.97-.81 2.72-2.1 1.32-3.57c-1.11-1.16-4.11.51-4.11.51l-17.17 6.71c-5.12 1.77-8.52 4.39-8.82 7.69c-.39 4.4 3.56 7.79 9.16 3.97z"
													fill="#f4b400"
												></path></g
											></svg
										>
									</svelte:fragment>
									<svelte:fragment slot="half">
										<svg
											viewBox="0 0 128 128"
											xmlns="http://www.w3.org/2000/svg"
											xmlns:xlink="http://www.w3.org/1999/xlink"
											aria-hidden="true"
											role="img"
											class="w-4 h-4 iconify iconify--noto"
											preserveAspectRatio="xMidYMid meet"
											fill="#000000"
											><g id="SVGRepo_bgCarrier" stroke-width="0"></g><g
												id="SVGRepo_tracerCarrier"
												stroke-linecap="round"
												stroke-linejoin="round"
											></g><g id="SVGRepo_iconCarrier"
												><path
													d="M68.05 7.23l13.46 30.7a7.047 7.047 0 0 0 5.82 4.19l32.79 2.94c3.71.54 5.19 5.09 2.5 7.71l-24.7 20.75c-2 1.68-2.91 4.32-2.36 6.87l7.18 33.61c.63 3.69-3.24 6.51-6.56 4.76L67.56 102a7.033 7.033 0 0 0-7.12 0l-28.62 16.75c-3.31 1.74-7.19-1.07-6.56-4.76l7.18-33.61c.54-2.55-.36-5.19-2.36-6.87L5.37 52.78c-2.68-2.61-1.2-7.17 2.5-7.71l32.79-2.94a7.047 7.047 0 0 0 5.82-4.19l13.46-30.7c1.67-3.36 6.45-3.36 8.11-.01z"
													fill="#fdd835"
												></path><path
													d="M67.07 39.77l-2.28-22.62c-.09-1.26-.35-3.42 1.67-3.42c1.6 0 2.47 3.33 2.47 3.33l6.84 18.16c2.58 6.91 1.52 9.28-.97 10.68c-2.86 1.6-7.08.35-7.73-6.13z"
													fill="#ffff8d"
												></path><path
													d="M95.28 71.51L114.9 56.2c.97-.81 2.72-2.1 1.32-3.57c-1.11-1.16-4.11.51-4.11.51l-17.17 6.71c-5.12 1.77-8.52 4.39-8.82 7.69c-.39 4.4 3.56 7.79 9.16 3.97z"
													fill="#f4b400"
												></path></g
											></svg
										>
									</svelte:fragment>
									<svelte:fragment slot="full">
										<svg
											viewBox="0 0 128 128"
											xmlns="http://www.w3.org/2000/svg"
											xmlns:xlink="http://www.w3.org/1999/xlink"
											aria-hidden="true"
											role="img"
											class="w-4 h-4 iconify iconify--noto"
											preserveAspectRatio="xMidYMid meet"
											fill="#000000"
											><g id="SVGRepo_bgCarrier" stroke-width="0"></g><g
												id="SVGRepo_tracerCarrier"
												stroke-linecap="round"
												stroke-linejoin="round"
											></g><g id="SVGRepo_iconCarrier"
												><path
													d="M68.05 7.23l13.46 30.7a7.047 7.047 0 0 0 5.82 4.19l32.79 2.94c3.71.54 5.19 5.09 2.5 7.71l-24.7 20.75c-2 1.68-2.91 4.32-2.36 6.87l7.18 33.61c.63 3.69-3.24 6.51-6.56 4.76L67.56 102a7.033 7.033 0 0 0-7.12 0l-28.62 16.75c-3.31 1.74-7.19-1.07-6.56-4.76l7.18-33.61c.54-2.55-.36-5.19-2.36-6.87L5.37 52.78c-2.68-2.61-1.2-7.17 2.5-7.71l32.79-2.94a7.047 7.047 0 0 0 5.82-4.19l13.46-30.7c1.67-3.36 6.45-3.36 8.11-.01z"
													fill="#fdd835"
												></path><path
													d="M67.07 39.77l-2.28-22.62c-.09-1.26-.35-3.42 1.67-3.42c1.6 0 2.47 3.33 2.47 3.33l6.84 18.16c2.58 6.91 1.52 9.28-.97 10.68c-2.86 1.6-7.08.35-7.73-6.13z"
													fill="#ffff8d"
												></path><path
													d="M95.28 71.51L114.9 56.2c.97-.81 2.72-2.1 1.32-3.57c-1.11-1.16-4.11.51-4.11.51l-17.17 6.71c-5.12 1.77-8.52 4.39-8.82 7.69c-.39 4.4 3.56 7.79 9.16 3.97z"
													fill="#f4b400"
												></path></g
											></svg
										>
									</svelte:fragment>
								</Ratings>
							</div>
						</div>
						<!-- price -->
						<div class="flex items-center justify-between">
							<p class="font-light">price</p>
							<p class="">${product.price}.00</p>
						</div>
					</div>

					<!-- info -->
					<div>
						<p class="w-10/12 text-sm font-light text-justify">
							{product.info}
						</p>
					</div>

					<!-- button -->
					<div
						class="flex items-center justify-center w-full 2xl:justify-start xl:justify-start lg:justify-start md:justify-start"
					>
						<a href={product.link}>
							<button
								class="px-16 py-3 text-sm font-semibold border-2 border-transparent rounded-md text-surface-100 bg-surface-600 hover:bg-white hover:border-2 hover:border-surface-600 hover:text-surface-600"
							>
								Buy Now
							</button>
						</a>
					</div>
				</div>
			{/each}
		</div>
	</div>
</div>
