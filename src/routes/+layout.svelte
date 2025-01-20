<script>
	import '../app.postcss';
	import { AppShell, AppBar } from '@skeletonlabs/skeleton';
	import { LightSwitch } from '@skeletonlabs/skeleton';
</script>

<!-- App Shell -->
<AppShell>
	<svelte:fragment slot="header">
		<!-- App Bar -->
		<div class="flex items-center justify-center w-full bg-surface-200 dark:bg-surface-900">
			<div
				class="grid w-full grid-cols-4 p-4 space-x-4 2xl:w-10/12 xl:w-10/12 lg:w-10/12 md:w-10/12 2xl:gap-x-0 xl:gap-x-0 lg:gap-x-0 md:gap-x-0 gap-x-4 bg-surface-200 dark:bg-surface-900"
			>
				<div
					class="relative flex items-center justify-start p-2 text-2xl w-fit crimson-text-regular"
				>
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
					<div class="absolute top-0.5 w-36 h-[1px] bg-warning-500 opacity-70"></div>
					<!-- bottom -->
					<div class="absolute bottom-0.5 w-36 h-[1px] bg-warning-500 opacity-70"></div>
					<!-- left -->
					<div class="absolute left-0.5 h-full w-[1px] bg-warning-500 opacity-70"></div>
					<!-- right -->
					<div class="absolute right-0.5 h-full w-[1px] bg-warning-500 opacity-70"></div>
					<p class="text-warning-500 dark:text-warning-500">AE</p>
					<p class="ml-3">Furnishers</p>
				</div>
				<div
					class="flex items-center justify-end w-full col-span-3 pr-8 space-x-6 2xl:pr-0 xl:pr-0 lg:pr-0 md:pr-0 2xl:justify-around xl:justify-around lg:justify-around md:justify-around 2xl:space-x-4 xl:space-x-4 lg:space-x-4 md:space-x-4"
				>
					<LightSwitch />
					{#each ['Home', 'About Us', 'Products', 'FAQ', 'Contact'] as link, i}
						<a
							class="font-medium transition-all duration-200 ease-in-out border-b-2 border-transparent text-surface-900 dark:text-surface-100 focus:text-warning-500 focus:border-warning-500 dark:focus:border-warning-500 hover:text-warning-500 dark:hover:text-warning-500 hover:border-warning-500
				{link === 'FAQ' || link === 'Contact' || link === 'About Us' ? 'hidden md:block' : ''}"
							href="#"
							target="_blank"
							rel="noreferrer"
						>
							{link}
						</a>
					{/each}
					<button
						class="hidden px-16 py-3 text-sm font-semibold transition-all duration-200 ease-in-out border-2 border-transparent rounded-md 2xl:block xl:block lg:block md:hidden text-surface-100 bg-surface-600 hover:bg-white hover:border-2 hover:border-surface-600 hover:text-surface-600"
					>
						Buy Now
					</button>
				</div>
			</div>
		</div>
	</svelte:fragment>
	<!-- Page Route Content -->
	<slot />

	<svelte:fragment slot="pageFooter">
		<div class="flex items-center justify-center w-full bg-surface-300">
			<div
				class="flex flex-col items-center justify-center w-full bg-surface-200 dark:bg-surface-900"
			>
				<div
					class="grid w-full grid-cols-4 p-4 space-x-4 2xl:w-10/12 xl:w-10/12 lg:w-10/12 md:w-10/12 2xl:gap-x-0 xl:gap-x-0 lg:gap-x-0 md:gap-x-0 gap-x-4 bg-surface-200 dark:bg-surface-900"
				>
					<div
						class="relative flex items-center justify-start col-span-2 p-2 text-2xl w-fit crimson-text-regular"
					>
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
						<div class="absolute top-0.5 w-36 h-[1px] bg-warning-500 opacity-70"></div>
						<!-- bottom -->
						<div class="absolute bottom-0.5 w-36 h-[1px] bg-warning-500 opacity-70"></div>
						<!-- left -->
						<div class="absolute left-0.5 h-full w-[1px] bg-warning-500 opacity-70"></div>
						<!-- right -->
						<div class="absolute right-0.5 h-full w-[1px] bg-warning-500 opacity-70"></div>
						<p class="text-warning-500 dark:text-warning-500">AE</p>
						<p class="ml-3">Furnishers</p>
					</div>
					<div
						class="flex items-center justify-end w-full col-span-2 pr-8 space-x-6 2xl:pr-0 xl:pr-0 lg:pr-0 md:pr-0 2xl:justify-around xl:justify-around lg:justify-around md:justify-around 2xl:space-x-4 xl:space-x-4 lg:space-x-4 md:space-x-4"
					>
						{#each ['Home', 'About Us', 'Products', 'FAQ', 'Contact'] as link, i}
							<a
								class="font-medium transition-all duration-200 ease-in-out border-b-2 border-transparent text-surface-900 dark:text-surface-100 focus:text-warning-500 focus:border-warning-500 dark:focus:border-warning-500 hover:text-warning-500 dark:hover:text-warning-500 hover:border-warning-500
					{link === 'FAQ' || link === 'About Us' ? 'hidden md:block' : ''}"
								href="#"
								target="_blank"
								rel="noreferrer"
							>
								{link}
							</a>
						{/each}
					</div>
				</div>
				<div class="w-10/12 h-[0.5px] bg-surface-800/70 dark:bg-surface-300/50"></div>
				<div
					class="grid w-full grid-cols-4 p-4 space-x-4 2xl:w-10/12 xl:w-10/12 lg:w-10/12 md:w-10/12 2xl:gap-x-0 xl:gap-x-0 lg:gap-x-0 md:gap-x-0 gap-x-4 bg-surface-200 dark:bg-surface-900"
				>
					<div class="flex items-center justify-start col-span-2">© 2025 AE Furnishers</div>
					<div class="flex items-center justify-end col-span-2 space-x-4">
						<!-- facebook -->
						<a
							class="flex items-center justify-center p-1 border-2 border-transparent rounded-full hover:bg-white hover:border-2 hover:border-surface-600 variant-glass-surface"
							href="https://www.facebook.com/"
							target="_blank"
						>
							<svg
								class="w-8 h-8"
								viewBox="0 0 48 48"
								fill="none"
								xmlns="http://www.w3.org/2000/svg"
								><g id="SVGRepo_bgCarrier" stroke-width="0"></g><g
									id="SVGRepo_tracerCarrier"
									stroke-linecap="round"
									stroke-linejoin="round"
								></g><g id="SVGRepo_iconCarrier">
									<circle cx="24" cy="24" r="20" fill="#3B5998"></circle>
									<path
										fill-rule="evenodd"
										clip-rule="evenodd"
										d="M29.315 16.9578C28.6917 16.8331 27.8498 16.74 27.3204 16.74C25.8867 16.74 25.7936 17.3633 25.7936 18.3607V20.1361H29.3774L29.065 23.8137H25.7936V35H21.3063V23.8137H19V20.1361H21.3063V17.8613C21.3063 14.7453 22.7708 13 26.4477 13C27.7252 13 28.6602 13.187 29.8753 13.4363L29.315 16.9578Z"
										fill="white"
									></path>
								</g></svg
							>
						</a>

						<!-- instagram -->
						<a
							class="flex items-center justify-center p-1 border-2 border-transparent rounded-full hover:bg-white hover:border-2 hover:border-surface-600 variant-glass-surface"
							href="https://www.instagram.com/"
							target="_blank"
						>
							<svg
								class="w-8 h-8"
								viewBox="0 0 32 32"
								fill="none"
								xmlns="http://www.w3.org/2000/svg"
								><g id="SVGRepo_bgCarrier" stroke-width="0"></g><g
									id="SVGRepo_tracerCarrier"
									stroke-linecap="round"
									stroke-linejoin="round"
								></g><g id="SVGRepo_iconCarrier">
									<rect x="2" y="2" width="28" height="28" rx="6" fill="url(#paint0_radial_87_7153)"
									></rect>
									<rect x="2" y="2" width="28" height="28" rx="6" fill="url(#paint1_radial_87_7153)"
									></rect>
									<rect x="2" y="2" width="28" height="28" rx="6" fill="url(#paint2_radial_87_7153)"
									></rect>
									<path
										d="M23 10.5C23 11.3284 22.3284 12 21.5 12C20.6716 12 20 11.3284 20 10.5C20 9.67157 20.6716 9 21.5 9C22.3284 9 23 9.67157 23 10.5Z"
										fill="white"
									></path>
									<path
										fill-rule="evenodd"
										clip-rule="evenodd"
										d="M16 21C18.7614 21 21 18.7614 21 16C21 13.2386 18.7614 11 16 11C13.2386 11 11 13.2386 11 16C11 18.7614 13.2386 21 16 21ZM16 19C17.6569 19 19 17.6569 19 16C19 14.3431 17.6569 13 16 13C14.3431 13 13 14.3431 13 16C13 17.6569 14.3431 19 16 19Z"
										fill="white"
									></path>
									<path
										fill-rule="evenodd"
										clip-rule="evenodd"
										d="M6 15.6C6 12.2397 6 10.5595 6.65396 9.27606C7.2292 8.14708 8.14708 7.2292 9.27606 6.65396C10.5595 6 12.2397 6 15.6 6H16.4C19.7603 6 21.4405 6 22.7239 6.65396C23.8529 7.2292 24.7708 8.14708 25.346 9.27606C26 10.5595 26 12.2397 26 15.6V16.4C26 19.7603 26 21.4405 25.346 22.7239C24.7708 23.8529 23.8529 24.7708 22.7239 25.346C21.4405 26 19.7603 26 16.4 26H15.6C12.2397 26 10.5595 26 9.27606 25.346C8.14708 24.7708 7.2292 23.8529 6.65396 22.7239C6 21.4405 6 19.7603 6 16.4V15.6ZM15.6 8H16.4C18.1132 8 19.2777 8.00156 20.1779 8.0751C21.0548 8.14674 21.5032 8.27659 21.816 8.43597C22.5686 8.81947 23.1805 9.43139 23.564 10.184C23.7234 10.4968 23.8533 10.9452 23.9249 11.8221C23.9984 12.7223 24 13.8868 24 15.6V16.4C24 18.1132 23.9984 19.2777 23.9249 20.1779C23.8533 21.0548 23.7234 21.5032 23.564 21.816C23.1805 22.5686 22.5686 23.1805 21.816 23.564C21.5032 23.7234 21.0548 23.8533 20.1779 23.9249C19.2777 23.9984 18.1132 24 16.4 24H15.6C13.8868 24 12.7223 23.9984 11.8221 23.9249C10.9452 23.8533 10.4968 23.7234 10.184 23.564C9.43139 23.1805 8.81947 22.5686 8.43597 21.816C8.27659 21.5032 8.14674 21.0548 8.0751 20.1779C8.00156 19.2777 8 18.1132 8 16.4V15.6C8 13.8868 8.00156 12.7223 8.0751 11.8221C8.14674 10.9452 8.27659 10.4968 8.43597 10.184C8.81947 9.43139 9.43139 8.81947 10.184 8.43597C10.4968 8.27659 10.9452 8.14674 11.8221 8.0751C12.7223 8.00156 13.8868 8 15.6 8Z"
										fill="white"
									></path>
									<defs>
										<radialGradient
											id="paint0_radial_87_7153"
											cx="0"
											cy="0"
											r="1"
											gradientUnits="userSpaceOnUse"
											gradientTransform="translate(12 23) rotate(-55.3758) scale(25.5196)"
										>
											<stop stop-color="#B13589"></stop>
											<stop offset="0.79309" stop-color="#C62F94"></stop>
											<stop offset="1" stop-color="#8A3AC8"></stop>
										</radialGradient>
										<radialGradient
											id="paint1_radial_87_7153"
											cx="0"
											cy="0"
											r="1"
											gradientUnits="userSpaceOnUse"
											gradientTransform="translate(11 31) rotate(-65.1363) scale(22.5942)"
										>
											<stop stop-color="#E0E8B7"></stop>
											<stop offset="0.444662" stop-color="#FB8A2E"></stop>
											<stop offset="0.71474" stop-color="#E2425C"></stop>
											<stop offset="1" stop-color="#E2425C" stop-opacity="0"></stop>
										</radialGradient>
										<radialGradient
											id="paint2_radial_87_7153"
											cx="0"
											cy="0"
											r="1"
											gradientUnits="userSpaceOnUse"
											gradientTransform="translate(0.500002 3) rotate(-8.1301) scale(38.8909 8.31836)"
										>
											<stop offset="0.156701" stop-color="#406ADC"></stop>
											<stop offset="0.467799" stop-color="#6A45BE"></stop>
											<stop offset="1" stop-color="#6A45BE" stop-opacity="0"></stop>
										</radialGradient>
									</defs>
								</g></svg
							>
						</a>
						<!-- twitter -->
						<a
							class="flex items-center justify-center p-1 border-2 border-transparent rounded-full hover:bg-white hover:border-2 hover:border-surface-600 variant-glass-surface"
							href=" https://www.twitter.com/"
							target="_blank"
						>
							<svg
								class="w-8 h-8"
								viewBox="0 0 48 48"
								fill="none"
								xmlns="http://www.w3.org/2000/svg"
								><g id="SVGRepo_bgCarrier" stroke-width="0"></g><g
									id="SVGRepo_tracerCarrier"
									stroke-linecap="round"
									stroke-linejoin="round"
								></g><g id="SVGRepo_iconCarrier">
									<circle cx="24" cy="24" r="20" fill="#1DA1F2"></circle>
									<path
										fill-rule="evenodd"
										clip-rule="evenodd"
										d="M36 16.3086C35.1177 16.7006 34.1681 16.9646 33.1722 17.0838C34.1889 16.4742 34.9697 15.5095 35.3368 14.36C34.3865 14.9247 33.3314 15.3335 32.2107 15.5551C31.3123 14.5984 30.0316 14 28.6165 14C25.8975 14 23.6928 16.2047 23.6928 18.9237C23.6928 19.3092 23.7368 19.6852 23.8208 20.046C19.7283 19.8412 16.1005 17.8805 13.6719 14.9015C13.2479 15.6287 13.0055 16.4742 13.0055 17.3766C13.0055 19.0845 13.8735 20.5916 15.1958 21.4747C14.3878 21.4491 13.6295 21.2275 12.9647 20.8587V20.9203C12.9647 23.3066 14.663 25.296 16.9141 25.7496C16.5013 25.8616 16.0661 25.9224 15.6174 25.9224C15.2998 25.9224 14.991 25.8912 14.6902 25.8336C15.3166 27.7895 17.1357 29.2134 19.2899 29.2534C17.6052 30.5733 15.4822 31.3612 13.1751 31.3612C12.7767 31.3612 12.3848 31.338 12 31.2916C14.1791 32.6884 16.7669 33.5043 19.5475 33.5043C28.6037 33.5043 33.5562 26.0016 33.5562 19.4956C33.5562 19.282 33.5522 19.0693 33.5418 18.8589C34.5049 18.1629 35.34 17.2958 36 16.3086Z"
										fill="white"
									></path>
								</g></svg
							>
						</a>
					</div>
				</div>
			</div>
		</div>
	</svelte:fragment>
</AppShell>

<style>
	@import url('https://fonts.googleapis.com/css2?family=Crimson+Text:ital,wght@0,400;0,600;0,700;1,400;1,600;1,700&display=swap');

	.crimson-text-regular {
		font-family: 'Crimson Text', serif;
		font-weight: 400;
		font-style: normal;
	}
</style>
