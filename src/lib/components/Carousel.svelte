<script>
	let slides = [
		{
			icon: '<svg version="1.1" id="Layer_1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" viewBox="0 0 512 512" xml:space="preserve" fill="#000000"><g id="SVGRepo_bgCarrier" stroke-width="0"></g><g id="SVGRepo_tracerCarrier" stroke-linecap="round" stroke-linejoin="round"></g><g id="SVGRepo_iconCarrier"> <path style="fill:#35bd32;" d="M256,0C177.328,82.672,46.672,64,46.672,64s0,92,0,224S256,512,256,512s209.328-92,209.328-224 s0-224,0-224S334.672,82.672,256,0z"></path> <polygon style="fill:#FFFFFF;" points="240.88,355.664 148.048,283.152 167.728,257.936 233.632,309.376 340.576,151.888 367.04,169.856 "></polygon> </g></svg>',
			title: 'Support',
			info: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Nam nemo a quos sit recusandae consequuntur.',
			buttonLink: '/products',
			color: 'green'
		},
		{
			icon: '<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg"><g id="SVGRepo_bgCarrier" stroke-width="0"></g><g id="SVGRepo_tracerCarrier" stroke-linecap="round" stroke-linejoin="round"></g><g id="SVGRepo_iconCarrier"> <path d="M17.5291 7.77C17.4591 7.76 17.3891 7.76 17.3191 7.77C15.7691 7.72 14.5391 6.45 14.5391 4.89C14.5391 3.3 15.8291 2 17.4291 2C19.0191 2 20.3191 3.29 20.3191 4.89C20.3091 6.45 19.0791 7.72 17.5291 7.77Z" fill="#9d438d"></path> <path d="M20.7916 14.7004C19.6716 15.4504 18.1016 15.7304 16.6516 15.5404C17.0316 14.7204 17.2316 13.8104 17.2416 12.8504C17.2416 11.8504 17.0216 10.9004 16.6016 10.0704C18.0816 9.8704 19.6516 10.1504 20.7816 10.9004C22.3616 11.9404 22.3616 13.6504 20.7916 14.7004Z" fill="#9d438d"></path> <path d="M6.44016 7.77C6.51016 7.76 6.58016 7.76 6.65016 7.77C8.20016 7.72 9.43016 6.45 9.43016 4.89C9.43016 3.29 8.14016 2 6.54016 2C4.95016 2 3.66016 3.29 3.66016 4.89C3.66016 6.45 4.89016 7.72 6.44016 7.77Z" fill="#9d438d"></path> <path d="M6.55109 12.8506C6.55109 13.8206 6.76109 14.7406 7.14109 15.5706C5.73109 15.7206 4.26109 15.4206 3.18109 14.7106C1.60109 13.6606 1.60109 11.9506 3.18109 10.9006C4.25109 10.1806 5.76109 9.89059 7.18109 10.0506C6.77109 10.8906 6.55109 11.8406 6.55109 12.8506Z" fill="#9d438d"></path> <path d="M12.1208 15.87C12.0408 15.86 11.9508 15.86 11.8608 15.87C10.0208 15.81 8.55078 14.3 8.55078 12.44C8.56078 10.54 10.0908 9 12.0008 9C13.9008 9 15.4408 10.54 15.4408 12.44C15.4308 14.3 13.9708 15.81 12.1208 15.87Z" fill="#9d438d"></path> <path d="M8.87078 17.9406C7.36078 18.9506 7.36078 20.6106 8.87078 21.6106C10.5908 22.7606 13.4108 22.7606 15.1308 21.6106C16.6408 20.6006 16.6408 18.9406 15.1308 17.9406C13.4208 16.7906 10.6008 16.7906 8.87078 17.9406Z" fill="#9d438d"></path> </g></svg>',
			title: 'Community',
			info: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Nam nemo a quos sit recusandae consequuntur.',
			buttonLink: '/products',
			color: 'purple'
		},
		{
			icon: '<svg viewBox="0 0 64 64" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" aria-hidden="true" role="img" class="iconify iconify--emojione" preserveAspectRatio="xMidYMid meet" fill="#000000"><g id="SVGRepo_bgCarrier" stroke-width="0"></g><g id="SVGRepo_tracerCarrier" stroke-linecap="round" stroke-linejoin="round"></g><g id="SVGRepo_iconCarrier"><path d="M62 25.2H39.1L32 3l-7.1 22.2H2l18.5 13.7l-7 22.1L32 47.3L50.5 61l-7.1-22.2L62 25.2z" fill="#ffce31"></path></g></svg>',
			title: 'Quality',
			info: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Nam nemo a quos sit recusandae consequuntur.',
			buttonLink: '/products',
			color: 'yellow'
		},
		{
			icon: '<svg version="1.1" id="Layer_1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" viewBox="0 0 512 512" xml:space="preserve" fill="#000000"><g id="SVGRepo_bgCarrier" stroke-width="0"></g><g id="SVGRepo_tracerCarrier" stroke-linecap="round" stroke-linejoin="round"></g><g id="SVGRepo_iconCarrier"> <path style="fill:#35bd32;" d="M256,0C177.328,82.672,46.672,64,46.672,64s0,92,0,224S256,512,256,512s209.328-92,209.328-224 s0-224,0-224S334.672,82.672,256,0z"></path> <polygon style="fill:#FFFFFF;" points="240.88,355.664 148.048,283.152 167.728,257.936 233.632,309.376 340.576,151.888 367.04,169.856 "></polygon> </g></svg>',
			title: 'Support',
			info: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Nam nemo a quos sit recusandae consequuntur.',
			buttonLink: '/products',
			color: 'green'
		},
		{
			icon: '<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg"><g id="SVGRepo_bgCarrier" stroke-width="0"></g><g id="SVGRepo_tracerCarrier" stroke-linecap="round" stroke-linejoin="round"></g><g id="SVGRepo_iconCarrier"> <path d="M17.5291 7.77C17.4591 7.76 17.3891 7.76 17.3191 7.77C15.7691 7.72 14.5391 6.45 14.5391 4.89C14.5391 3.3 15.8291 2 17.4291 2C19.0191 2 20.3191 3.29 20.3191 4.89C20.3091 6.45 19.0791 7.72 17.5291 7.77Z" fill="#9d438d"></path> <path d="M20.7916 14.7004C19.6716 15.4504 18.1016 15.7304 16.6516 15.5404C17.0316 14.7204 17.2316 13.8104 17.2416 12.8504C17.2416 11.8504 17.0216 10.9004 16.6016 10.0704C18.0816 9.8704 19.6516 10.1504 20.7816 10.9004C22.3616 11.9404 22.3616 13.6504 20.7916 14.7004Z" fill="#9d438d"></path> <path d="M6.44016 7.77C6.51016 7.76 6.58016 7.76 6.65016 7.77C8.20016 7.72 9.43016 6.45 9.43016 4.89C9.43016 3.29 8.14016 2 6.54016 2C4.95016 2 3.66016 3.29 3.66016 4.89C3.66016 6.45 4.89016 7.72 6.44016 7.77Z" fill="#9d438d"></path> <path d="M6.55109 12.8506C6.55109 13.8206 6.76109 14.7406 7.14109 15.5706C5.73109 15.7206 4.26109 15.4206 3.18109 14.7106C1.60109 13.6606 1.60109 11.9506 3.18109 10.9006C4.25109 10.1806 5.76109 9.89059 7.18109 10.0506C6.77109 10.8906 6.55109 11.8406 6.55109 12.8506Z" fill="#9d438d"></path> <path d="M12.1208 15.87C12.0408 15.86 11.9508 15.86 11.8608 15.87C10.0208 15.81 8.55078 14.3 8.55078 12.44C8.56078 10.54 10.0908 9 12.0008 9C13.9008 9 15.4408 10.54 15.4408 12.44C15.4308 14.3 13.9708 15.81 12.1208 15.87Z" fill="#9d438d"></path> <path d="M8.87078 17.9406C7.36078 18.9506 7.36078 20.6106 8.87078 21.6106C10.5908 22.7606 13.4108 22.7606 15.1308 21.6106C16.6408 20.6006 16.6408 18.9406 15.1308 17.9406C13.4208 16.7906 10.6008 16.7906 8.87078 17.9406Z" fill="#9d438d"></path> </g></svg>',
			title: 'Community5',
			info: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Nam nemo a quos sit recusandae consequuntur.',
			buttonLink: '/products',
			color: 'purple'
		}
	];

	let currentSlide = 0;

	// Auto-slide every 5 seconds
	let autoSlide = setInterval(() => {
		nextSlide();
	}, 5000);

	function nextSlide() {
		currentSlide = (currentSlide + 1) % slides.length;
		console.log('Next Slide:', currentSlide);
	}

	function prevSlide() {
		currentSlide = (currentSlide - 1 + slides.length) % slides.length;
		console.log('Previous Slide:', currentSlide);
	}
	function isVisible(index) {
		const visibleIndexes = [
			currentSlide,
			(currentSlide + 1) % slides.length,
			(currentSlide + 2) % slides.length
		];
		console.log('Visible Indices:', visibleIndexes);
		return visibleIndexes.includes(index);
	}
	// Pause auto-slide on hover
	function pauseSlide() {
		clearInterval(autoSlide);
	}

	function resumeSlide() {
		autoSlide = setInterval(() => {
			nextSlide();
		}, 5000);
	}
</script>

<!-- carousel -->
<div
	class="grid grid-cols-3 space-x-4 mt-10 m-auto relative max-w-[1000px]"
	on:mouseenter={pauseSlide}
	on:mouseleave={resumeSlide}
	role="region"
	aria-label="Carousel"
>
	<!-- cards -->
	{#each slides as slide, index}
		<div
			class="transition-transform rounded-md shadow-lg bg-surface-300 dark:bg-surface-900 hover:scale-105 hover:shadow-2xl"
			class:hidden={!isVisible(index)}
		>
			<div class="p-10 space-y-3">
				<!-- icon -->
				<div class="w-10 h-10 p-1.5 rounded-full" style="background-color: {slide.color};">
					{@html slide.icon}
				</div>
				<!-- title -->
				<div>
					{slide.title}
				</div>
				<!-- info -->
				<div class="w-11/12 text-sm font-light text-justify">
					{slide.info}
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
	{/each}

	<!-- arrows -->
	<!-- right arrow -->
	<button
		on:click={() => nextSlide()}
		class="p-1.5 rounded-full variant-glass-surface h-fit w-fit absolute top-1/2 -right-12 transform -translate-y-1/2"
		aria-label="Next Slide"
	>
		<svg class="w-5 h-5" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
			<path
				d="M9 5L14.15 10C14.4237 10.2563 14.6419 10.5659 14.791 10.9099C14.9402 11.2539 15.0171 11.625 15.0171 12C15.0171 12.375 14.9402 12.7458 14.791 13.0898C14.6419 13.4339 14.4237 13.7437 14.15 14L9 19"
				stroke="#c7c7c7"
				stroke-width="1.5"
				stroke-linecap="round"
				stroke-linejoin="round"
			></path>
		</svg>
	</button>

	<!-- left arrow -->
	<button
		on:click={() => prevSlide()}
		class="p-1.5 rounded-full variant-glass-surface h-fit w-fit absolute top-1/2 -left-16 transform -translate-y-1/2"
		aria-label="Previous Slide"
	>
		<svg class="w-5 h-5" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
			<path
				d="M14.9991 19L9.83911 14C9.56672 13.7429 9.34974 13.433 9.20142 13.0891C9.0531 12.7452 8.97656 12.3745 8.97656 12C8.97656 11.6255 9.0531 11.2548 9.20142 10.9109C9.34974 10.567 9.56672 10.2571 9.83911 10L14.9991 5"
				stroke="#c7c7c7"
				stroke-width="1.5"
				stroke-linecap="round"
				stroke-linejoin="round"
			></path>
		</svg>
	</button>
</div>

<style>
	.hidden {
		display: none;
	}
	button {
		z-index: 20; /* Ensure the buttons are on top */
	}
</style>
