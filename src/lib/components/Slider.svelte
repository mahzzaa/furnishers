<script>
	// @ts-ignore
	import { blur, slide } from 'svelte/transition';

	export let duration;
	export let slides;

	let currentSlide = 0;
	const nextSlide = () => {
		currentSlide++;
		if (currentSlide >= slides.length) {
			currentSlide = 0;
		}
		timer();
	};

	const prevSlide = () => {
		currentSlide--;
		if (currentSlide <= 0) {
			currentSlide = slides.length - 1;
		}
		timer();
	};

	// @ts-ignore
	const goToSlide = (index) => {
		currentSlide = index;
		timer();
	};

	let interval;
	const timer = () => {
		interval = setInterval(nextSlide, duration);
	};
	timer();
</script>

<div class="slider w-[90vw] h-[300px] relative">
	{#each slides as slider, i}
		{#if currentSlide === i}
			<div
				class="absolute inset-0 flex items-center justify-center rounded-md slide"
				transition:blur={{ amount: 5 }}
			>
				<div
					class="transition-transform rounded-md shadow-lg bg-surface-300 dark:bg-surface-900 hover:scale-105 hover:shadow-2xl"
				>
					<div class="z-40 p-10 space-y-3 bg-surface-800">
						<!-- icon -->
						<div class="w-10 h-10 p-1.5 rounded-full" style="background-color: {slider.color};">
							{@html slider.icon}
						</div>
						<!-- title -->
						<div>
							{slider.title}
						</div>
						<!-- info -->
						<div class="w-11/12 text-sm font-light text-justify">
							{slider.info}
						</div>
						<!-- button -->
						<div
							class="flex items-center justify-center w-full 2xl:justify-start xl:justify-start lg:justify-start md:justify-center"
						>
							<button
								class="px-4 py-2 text-xs font-semibold border-2 border-transparent rounded-md text-surface-100 bg-surface-600 hover:bg-white hover:border-2 hover:border-surface-600 hover:text-surface-600"
							>
								Sign up
							</button>
						</div>
					</div>
				</div>
			</div>
		{/if}
	{/each}
	<button
		class="next absolute z-20 top-1/2 -translate-y-1/2 2xl:right-[20px] xl:right-[20px] lg:right-[20px] md:right-[20px] right-0 cursor-pointer"
		on:click={nextSlide}
	>
		<svg class="w-8 h-8" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg"
			><g id="SVGRepo_bgCarrier" stroke-width="0"></g><g
				id="SVGRepo_tracerCarrier"
				stroke-linecap="round"
				stroke-linejoin="round"
			></g><g id="SVGRepo_iconCarrier">
				<path
					d="M9 5L14.15 10C14.4237 10.2563 14.6419 10.5659 14.791 10.9099C14.9402 11.2539 15.0171 11.625 15.0171 12C15.0171 12.375 14.9402 12.7458 14.791 13.0898C14.6419 13.4339 14.4237 13.7437 14.15 14L9 19"
					stroke="#c7c7c7"
					stroke-width="1.5"
					stroke-linecap="round"
					stroke-linejoin="round"
				></path>
			</g></svg
		>
	</button>
	<button
		class="absolute z-20 -translate-y-1/2 prev top-1/2 2xl:left-[20px] xl:left-[20px] lg:left-[20px] md:left-[20px] left-0 cursor-pointer"
		on:click={prevSlide}
	>
		<svg class="w-8 h-8" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg"
			><g id="SVGRepo_bgCarrier" stroke-width="0"></g><g
				id="SVGRepo_tracerCarrier"
				stroke-linecap="round"
				stroke-linejoin="round"
			></g><g id="SVGRepo_iconCarrier">
				<path
					d="M14.9991 19L9.83911 14C9.56672 13.7429 9.34974 13.433 9.20142 13.0891C9.0531 12.7452 8.97656 12.3745 8.97656 12C8.97656 11.6255 9.0531 11.2548 9.20142 10.9109C9.34974 10.567 9.56672 10.2571 9.83911 10L14.9991 5"
					stroke="#c7c7c7"
					stroke-width="1.5"
					stroke-linecap="round"
					stroke-linejoin="round"
				></path>
			</g></svg
		>
	</button>

	<div
		class="nav absolute -bottom-10 left-0 right-0 h-[50px] z-20 flex justify-evenly items-center"
	>
		{#each slides as slider, i}
			<button
				on:click={() => goToSlide(i)}
				class:current={i === currentSlide}
				class:onedown={i === currentSlide - 1}
				class:twodown={i === currentSlide - 2}
				class:oneup={i === currentSlide + 1}
				class:twoup={i === currentSlide + 2}
				class="bubble bg-white p-0 border-0 h-[20px] w-[10px] rounded-full cursor-pointer transition-all duration-300 ease-out opacity-20"
			>
			</button>
		{/each}
	</div>
</div>

<style>
	.current {
		height: 20px;
		opacity: 0.8;
	}
	.onedown,
	.oneup {
		height: 10px;
	}
	.twodown,
	.twoup {
		height: 5px;
	}
</style>
