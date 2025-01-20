<script>
	import networkDots from '../assets/network-dots.png';
	import Slider from './Slider.svelte';
	let slides = [
		{
			index: 0,
			icon: '<svg version="1.1" id="Layer_1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" viewBox="0 0 512 512" xml:space="preserve" fill="#000000"><g id="SVGRepo_bgCarrier" stroke-width="0"></g><g id="SVGRepo_tracerCarrier" stroke-linecap="round" stroke-linejoin="round"></g><g id="SVGRepo_iconCarrier"> <path style="fill:#35bd32;" d="M256,0C177.328,82.672,46.672,64,46.672,64s0,92,0,224S256,512,256,512s209.328-92,209.328-224 s0-224,0-224S334.672,82.672,256,0z"></path> <polygon style="fill:#FFFFFF;" points="240.88,355.664 148.048,283.152 167.728,257.936 233.632,309.376 340.576,151.888 367.04,169.856 "></polygon> </g></svg>',
			title: 'Support',
			info: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Nam nemo a quos sit recusandae consequuntur.',
			buttonLink: '/products',
			color: 'green'
		},
		{
			index: 1,
			icon: '<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg"><g id="SVGRepo_bgCarrier" stroke-width="0"></g><g id="SVGRepo_tracerCarrier" stroke-linecap="round" stroke-linejoin="round"></g><g id="SVGRepo_iconCarrier"> <path d="M17.5291 7.77C17.4591 7.76 17.3891 7.76 17.3191 7.77C15.7691 7.72 14.5391 6.45 14.5391 4.89C14.5391 3.3 15.8291 2 17.4291 2C19.0191 2 20.3191 3.29 20.3191 4.89C20.3091 6.45 19.0791 7.72 17.5291 7.77Z" fill="#9d438d"></path> <path d="M20.7916 14.7004C19.6716 15.4504 18.1016 15.7304 16.6516 15.5404C17.0316 14.7204 17.2316 13.8104 17.2416 12.8504C17.2416 11.8504 17.0216 10.9004 16.6016 10.0704C18.0816 9.8704 19.6516 10.1504 20.7816 10.9004C22.3616 11.9404 22.3616 13.6504 20.7916 14.7004Z" fill="#9d438d"></path> <path d="M6.44016 7.77C6.51016 7.76 6.58016 7.76 6.65016 7.77C8.20016 7.72 9.43016 6.45 9.43016 4.89C9.43016 3.29 8.14016 2 6.54016 2C4.95016 2 3.66016 3.29 3.66016 4.89C3.66016 6.45 4.89016 7.72 6.44016 7.77Z" fill="#9d438d"></path> <path d="M6.55109 12.8506C6.55109 13.8206 6.76109 14.7406 7.14109 15.5706C5.73109 15.7206 4.26109 15.4206 3.18109 14.7106C1.60109 13.6606 1.60109 11.9506 3.18109 10.9006C4.25109 10.1806 5.76109 9.89059 7.18109 10.0506C6.77109 10.8906 6.55109 11.8406 6.55109 12.8506Z" fill="#9d438d"></path> <path d="M12.1208 15.87C12.0408 15.86 11.9508 15.86 11.8608 15.87C10.0208 15.81 8.55078 14.3 8.55078 12.44C8.56078 10.54 10.0908 9 12.0008 9C13.9008 9 15.4408 10.54 15.4408 12.44C15.4308 14.3 13.9708 15.81 12.1208 15.87Z" fill="#9d438d"></path> <path d="M8.87078 17.9406C7.36078 18.9506 7.36078 20.6106 8.87078 21.6106C10.5908 22.7606 13.4108 22.7606 15.1308 21.6106C16.6408 20.6006 16.6408 18.9406 15.1308 17.9406C13.4208 16.7906 10.6008 16.7906 8.87078 17.9406Z" fill="#9d438d"></path> </g></svg>',
			title: 'Community',
			info: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Nam nemo a quos sit recusandae consequuntur.',
			buttonLink: '/products',
			color: 'purple'
		},
		{
			index: 2,
			icon: '<svg viewBox="0 0 64 64" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" aria-hidden="true" role="img" class="iconify iconify--emojione" preserveAspectRatio="xMidYMid meet" fill="#000000"><g id="SVGRepo_bgCarrier" stroke-width="0"></g><g id="SVGRepo_tracerCarrier" stroke-linecap="round" stroke-linejoin="round"></g><g id="SVGRepo_iconCarrier"><path d="M62 25.2H39.1L32 3l-7.1 22.2H2l18.5 13.7l-7 22.1L32 47.3L50.5 61l-7.1-22.2L62 25.2z" fill="#ffce31"></path></g></svg>',
			title: 'Quality',
			info: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Nam nemo a quos sit recusandae consequuntur.',
			buttonLink: '/products',
			color: 'yellow'
		},
		{
			index: 3,
			icon: '<svg version="1.1" id="Layer_1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" viewBox="0 0 512 512" xml:space="preserve" fill="#000000"><g id="SVGRepo_bgCarrier" stroke-width="0"></g><g id="SVGRepo_tracerCarrier" stroke-linecap="round" stroke-linejoin="round"></g><g id="SVGRepo_iconCarrier"> <path style="fill:#35bd32;" d="M256,0C177.328,82.672,46.672,64,46.672,64s0,92,0,224S256,512,256,512s209.328-92,209.328-224 s0-224,0-224S334.672,82.672,256,0z"></path> <polygon style="fill:#FFFFFF;" points="240.88,355.664 148.048,283.152 167.728,257.936 233.632,309.376 340.576,151.888 367.04,169.856 "></polygon> </g></svg>',
			title: 'Support',
			info: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Nam nemo a quos sit recusandae consequuntur.',
			buttonLink: '/products',
			color: 'green'
		},
		{
			index: 4,
			icon: '<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg"><g id="SVGRepo_bgCarrier" stroke-width="0"></g><g id="SVGRepo_tracerCarrier" stroke-linecap="round" stroke-linejoin="round"></g><g id="SVGRepo_iconCarrier"> <path d="M17.5291 7.77C17.4591 7.76 17.3891 7.76 17.3191 7.77C15.7691 7.72 14.5391 6.45 14.5391 4.89C14.5391 3.3 15.8291 2 17.4291 2C19.0191 2 20.3191 3.29 20.3191 4.89C20.3091 6.45 19.0791 7.72 17.5291 7.77Z" fill="#9d438d"></path> <path d="M20.7916 14.7004C19.6716 15.4504 18.1016 15.7304 16.6516 15.5404C17.0316 14.7204 17.2316 13.8104 17.2416 12.8504C17.2416 11.8504 17.0216 10.9004 16.6016 10.0704C18.0816 9.8704 19.6516 10.1504 20.7816 10.9004C22.3616 11.9404 22.3616 13.6504 20.7916 14.7004Z" fill="#9d438d"></path> <path d="M6.44016 7.77C6.51016 7.76 6.58016 7.76 6.65016 7.77C8.20016 7.72 9.43016 6.45 9.43016 4.89C9.43016 3.29 8.14016 2 6.54016 2C4.95016 2 3.66016 3.29 3.66016 4.89C3.66016 6.45 4.89016 7.72 6.44016 7.77Z" fill="#9d438d"></path> <path d="M6.55109 12.8506C6.55109 13.8206 6.76109 14.7406 7.14109 15.5706C5.73109 15.7206 4.26109 15.4206 3.18109 14.7106C1.60109 13.6606 1.60109 11.9506 3.18109 10.9006C4.25109 10.1806 5.76109 9.89059 7.18109 10.0506C6.77109 10.8906 6.55109 11.8406 6.55109 12.8506Z" fill="#9d438d"></path> <path d="M12.1208 15.87C12.0408 15.86 11.9508 15.86 11.8608 15.87C10.0208 15.81 8.55078 14.3 8.55078 12.44C8.56078 10.54 10.0908 9 12.0008 9C13.9008 9 15.4408 10.54 15.4408 12.44C15.4308 14.3 13.9708 15.81 12.1208 15.87Z" fill="#9d438d"></path> <path d="M8.87078 17.9406C7.36078 18.9506 7.36078 20.6106 8.87078 21.6106C10.5908 22.7606 13.4108 22.7606 15.1308 21.6106C16.6408 20.6006 16.6408 18.9406 15.1308 17.9406C13.4208 16.7906 10.6008 16.7906 8.87078 17.9406Z" fill="#9d438d"></path> </g></svg>',
			title: 'Community5',
			info: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Nam nemo a quos sit recusandae consequuntur.',
			buttonLink: '/products',
			color: 'purple'
		},
		{
			index: 5,
			icon: '<svg viewBox="0 0 1024 1024" class="icon" version="1.1" xmlns="http://www.w3.org/2000/svg" fill="#000000"><g id="SVGRepo_bgCarrier" stroke-width="0"></g><g id="SVGRepo_tracerCarrier" stroke-linecap="round" stroke-linejoin="round"></g><g id="SVGRepo_iconCarrier"><path d="M512 469.333333m-426.666667 0a426.666667 426.666667 0 1 0 853.333334 0 426.666667 426.666667 0 1 0-853.333334 0Z" fill="#FFF59D"></path><path d="M789.333333 469.333333c0-164.266667-140.8-294.4-309.333333-275.2-128 14.933333-230.4 117.333333-243.2 245.333334-10.666667 98.133333 29.866667 185.6 98.133333 241.066666 29.866667 25.6 49.066667 61.866667 49.066667 102.4v6.4h256v-2.133333c0-38.4 17.066667-76.8 46.933333-102.4 61.866667-51.2 102.4-128 102.4-215.466667z" fill="#FBC02D"></path><path d="M652.8 430.933333l-64-42.666666c-6.4-4.266667-17.066667-4.266667-23.466667 0L512 422.4l-51.2-34.133333c-6.4-4.266667-17.066667-4.266667-23.466667 0l-64 42.666666c-4.266667 4.266667-8.533333 8.533333-8.533333 14.933334s0 12.8 4.266667 17.066666l81.066666 100.266667V789.333333h42.666667V554.666667c0-4.266667-2.133333-8.533333-4.266667-12.8l-70.4-87.466667 32-21.333333 51.2 34.133333c6.4 4.266667 17.066667 4.266667 23.466667 0l51.2-34.133333 32 21.333333-70.4 87.466667c-2.133333 4.266667-4.266667 8.533333-4.266667 12.8v234.666666h42.666667V563.2l81.066667-100.266667c4.266667-4.266667 6.4-10.666667 4.266666-17.066666s-4.266667-12.8-8.533333-14.933334z" fill="#FFF59D"></path><path d="M512 938.666667m-64 0a64 64 0 1 0 128 0 64 64 0 1 0-128 0Z" fill="#5C6BC0"></path><path d="M554.666667 960h-85.333334c-46.933333 0-85.333333-38.4-85.333333-85.333333v-106.666667h256v106.666667c0 46.933333-38.4 85.333333-85.333333 85.333333z" fill="#9FA8DA"></path><path d="M640 874.666667l-247.466667 34.133333c6.4 14.933333 19.2 29.866667 34.133334 38.4l200.533333-27.733333c8.533333-12.8 12.8-27.733333 12.8-44.8zM384 825.6v42.666667L640 832v-42.666667z" fill="#5C6BC0"></path></g></svg>',
			title: 'Support',
			info: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Nam nemo a quos sit recusandae consequuntur.',
			buttonLink: '/products',
			color: 'yellow'
		},
		{
			index: 6,
			icon: '<svg viewBox="0 0 1024 1024" class="icon" version="1.1" xmlns="http://www.w3.org/2000/svg" fill="#000000"><g id="SVGRepo_bgCarrier" stroke-width="0"></g><g id="SVGRepo_tracerCarrier" stroke-linecap="round" stroke-linejoin="round"></g><g id="SVGRepo_iconCarrier"><path d="M512 64l100.266667 76.8 123.733333-17.066667 46.933333 117.333334 117.333334 46.933333-17.066667 123.733333L960 512l-76.8 100.266667 17.066667 123.733333-117.333334 46.933333-46.933333 117.333334-123.733333-17.066667L512 960l-100.266667-76.8-123.733333 17.066667-46.933333-117.333334-117.333334-46.933333 17.066667-123.733333L64 512l76.8-100.266667-17.066667-123.733333 117.333334-46.933333 46.933333-117.333334 123.733333 17.066667z" fill="#8BC34A"></path><path d="M738.133333 311.466667L448 601.6l-119.466667-119.466667-59.733333 59.733334 179.2 179.2 349.866667-349.866667z" fill="#CCFF90"></path></g></svg>',
			title: 'Community5',
			info: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Nam nemo a quos sit recusandae consequuntur.',
			buttonLink: '/products',
			color: 'green'
		}
	];
</script>

<div
	class="relative z-0 flex flex-col items-center justify-center w-full h-full py-20 overflow-hidden bg-surface-200 dark:bg-surface-700"
>
	<img
		class="absolute top-0 h-full -right-10 w-[600px] opacity-50 -z-10 rotate-180"
		src={networkDots}
		alt="network-dots"
	/>
	<img
		class="absolute -top-10 h-[120%] -right-10 w-[500px] opacity-20 -z-10 rotate-180"
		src={networkDots}
		alt="network-dots"
	/>
	<div class="flex flex-col items-center justify-center space-y-5">
		<!-- Title -->
		<div
			class="flex items-center justify-center space-x-2 text-4xl font-semibold tracking-wide text-surface-600 dark:text-surface-100"
		>
			<p>Why</p>
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

				<p class="px-3 py-2">Choose US?</p>
			</div>
		</div>
		<!-- info -->
		<p class="px-5 text-sm font-light text-center">
			Lorem ipsum dolor sit amet consectetur adipisicing elit. Nam nemo a quos sit recusandae
			consequuntur.
		</p>
	</div>
	<div class="mt-10">
		<Slider duration={3000} {slides} />
	</div>
</div>
