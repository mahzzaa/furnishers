<script>
	import { Ratings } from '@skeletonlabs/skeleton';
	import networkDots from '../assets/network-dots.png';

	let happyClients = [
		{
			avatar: 'https://i.pinimg.com/736x/b6/a9/8b/b6a98bca5933e5827e114ae7b63300db.jpg',
			name: 'John Doe',
			bio: 'architect',
			stars: 5,
			comment:
				'lorem ipsum dolor sit amet consectetur adipisicing elit. Nam nemo a quos sit recusandae consequuntur.'
		},
		{
			avatar: 'https://i.pinimg.com/736x/8a/bf/bd/8abfbd075311d1f0320ae3cf88c4356e.jpg',
			name: 'David Smith',
			bio: 'inner designer',
			stars: 3,
			comment:
				'lorem ipsum dolor sit amet consectetur adipisicing elit. Nam nemo a quos sit recusandae consequuntur.'
		},
		{
			avatar: 'https://i.pinimg.com/736x/4c/31/ca/4c31ca4229f3240ec02151da4c21f888.jpg',
			name: 'Alice Bob',
			bio: 'decorator',
			stars: 5,
			comment:
				'lorem ipsum dolor sit amet consectetur adipisicing elit. Nam nemo a quos sit recusandae consequuntur.'
		}
	];
</script>

<div
	class="relative z-0 flex flex-col items-center justify-center w-full h-full py-20 space-y-8 overflow-hidden bg-surface-200 dark:bg-surface-700"
>
	<!-- backgorund image -->

	<img
		class="absolute 2xl:block xl:block lg:block md:block hidden top-0 h-full -left-10 w-[600px] opacity-50 -z-10"
		src={networkDots}
		alt="network-dots"
	/>
	<img
		class="absolute 2xl:block xl:block lg:block md:block hidden -top-10 h-[120%] -left-10 w-[500px] opacity-20 -z-10"
		src={networkDots}
		alt="network-dots"
	/>

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

			<p class="px-3 py-2">Happy Client</p>
		</div>
	</div>

	<!-- info -->
	<div class="w-4/5 2xl:w-full xl:w-full lg:w-full md:w-full">
		<p class="text-sm font-light text-center">
			Lorem ipsum dolor sit amet consectetur adipisicing elit. Nam nemo a quos sit recusandae
			consequuntur.
		</p>
	</div>

	<!-- cards -->
	<div
		class="grid w-4/5 grid-cols-1 2xl:w-4/5 xl:w-4/5 lg:w-4/5 md:11/12 2xl:grid-cols-3 xl:grid-cols-3 lg:grid-cols-3 md:grid-cols-3 2xl:gap-x-5 xl:gap-x-5 lg:gap-x-5 md:gap-x-5 gap-x-0 2xl:gap-y-0 xl:gap-y-0 lg:gap-y-0 md:gap-y-0 gap-y-5"
	>
		{#each happyClients as happyClient}
			<div
				class="relative z-30 p-10 space-y-3 transition-transform rounded-md shadow-lg 2xl:p-10 xl:p-10 lg:p-10 md:p-8 bg-surface-300 dark:bg-surface-900 hover:scale-105 hover:shadow-2xl"
			>
				<!-- decoration -->
				<div class="absolute top-3 left-3">
					<svg
						class="block w-10 h-10 dark:hidden"
						fill="#000000"
						viewBox="0 0 64 64"
						version="1.1"
						xmlns="http://www.w3.org/2000/svg"
						xmlns:xlink="http://www.w3.org/1999/xlink"
						xml:space="preserve"
						xmlns:serif="http://www.serif.com/"
						style="fill-rule:evenodd;clip-rule:evenodd;stroke-linejoin:round;stroke-miterlimit:2;"
						><g id="SVGRepo_bgCarrier" stroke-width="0"></g><g
							id="SVGRepo_tracerCarrier"
							stroke-linecap="round"
							stroke-linejoin="round"
						></g><g id="SVGRepo_iconCarrier">
							<rect id="Icons" x="-640" y="0" width="1280" height="800" style="fill:none;"></rect>
							<g id="Icons1" serif:id="Icons">
								<g id="Strike"> </g> <g id="H1"> </g> <g id="H2"> </g> <g id="H3"> </g>
								<g id="list-ul"> </g> <g id="hamburger-1"> </g> <g id="hamburger-2"> </g>
								<g id="list-ol"> </g> <g id="list-task"> </g>
								<path
									id="quote-1"
									d="M27.194,12l0,8.025c-2.537,0.14 -4.458,0.603 -5.761,1.39c-1.304,0.787 -2.22,2.063 -2.749,3.829c-0.528,1.766 -0.793,4.292 -0.793,7.579l9.303,0l0,19.145l-19.081,0l0,-18.201c0,-7.518 1.612,-13.025 4.836,-16.522c3.225,-3.497 7.973,-5.245 14.245,-5.245Zm28.806,0l0,8.025c-2.537,0.14 -4.457,0.586 -5.761,1.338c-1.304,0.751 -2.247,2.028 -2.828,3.829c-0.581,1.8 -0.872,4.344 -0.872,7.631l9.461,0l0,19.145l-19.186,0l0,-18.201c0,-7.518 1.603,-13.025 4.809,-16.522c3.207,-3.497 7.999,-5.245 14.377,-5.245Z"
									style="fill-rule:nonzero;"
								></path> <g id="trash"> </g> <g id="vertical-menu"> </g>
								<g id="horizontal-menu"> </g> <g id="sidebar-2"> </g> <g id="Pen"> </g>
								<g id="Pen1" serif:id="Pen"> </g> <g id="clock"> </g> <g id="external-link"> </g>
								<g id="hr"> </g> <g id="info"> </g> <g id="warning"> </g> <g id="plus-circle"> </g>
								<g id="minus-circle"> </g> <g id="vue"> </g> <g id="cog"> </g> <g id="logo"> </g>
								<g id="radio-check"> </g> <g id="eye-slash"> </g> <g id="eye"> </g>
								<g id="toggle-off"> </g> <g id="shredder"> </g>
								<g id="spinner--loading--dots-" serif:id="spinner [loading, dots]"> </g>
								<g id="react"> </g> <g id="check-selected"> </g> <g id="turn-off"> </g>
								<g id="code-block"> </g> <g id="user"> </g> <g id="coffee-bean"> </g>
								<g id="coffee-beans"> <g id="coffee-bean1" serif:id="coffee-bean"> </g> </g>
								<g id="coffee-bean-filled"> </g>
								<g id="coffee-beans-filled"> <g id="coffee-bean2" serif:id="coffee-bean"> </g> </g>
								<g id="clipboard"> </g> <g id="clipboard-paste"> </g> <g id="clipboard-copy"> </g>
								<g id="Layer1"> </g>
							</g>
						</g></svg
					>
					<svg
						class="hidden w-10 h-10 dark:block"
						fill="#ffffff"
						viewBox="0 0 64 64"
						version="1.1"
						xmlns="http://www.w3.org/2000/svg"
						xmlns:xlink="http://www.w3.org/1999/xlink"
						xml:space="preserve"
						xmlns:serif="http://www.serif.com/"
						style="fill-rule:evenodd;clip-rule:evenodd;stroke-linejoin:round;stroke-miterlimit:2;"
						><g id="SVGRepo_bgCarrier" stroke-width="0"></g><g
							id="SVGRepo_tracerCarrier"
							stroke-linecap="round"
							stroke-linejoin="round"
						></g><g id="SVGRepo_iconCarrier">
							<rect id="Icons" x="-640" y="0" width="1280" height="800" style="fill:none;"></rect>
							<g id="Icons1" serif:id="Icons">
								<g id="Strike"> </g> <g id="H1"> </g> <g id="H2"> </g> <g id="H3"> </g>
								<g id="list-ul"> </g> <g id="hamburger-1"> </g> <g id="hamburger-2"> </g>
								<g id="list-ol"> </g> <g id="list-task"> </g>
								<path
									id="quote-1"
									d="M27.194,12l0,8.025c-2.537,0.14 -4.458,0.603 -5.761,1.39c-1.304,0.787 -2.22,2.063 -2.749,3.829c-0.528,1.766 -0.793,4.292 -0.793,7.579l9.303,0l0,19.145l-19.081,0l0,-18.201c0,-7.518 1.612,-13.025 4.836,-16.522c3.225,-3.497 7.973,-5.245 14.245,-5.245Zm28.806,0l0,8.025c-2.537,0.14 -4.457,0.586 -5.761,1.338c-1.304,0.751 -2.247,2.028 -2.828,3.829c-0.581,1.8 -0.872,4.344 -0.872,7.631l9.461,0l0,19.145l-19.186,0l0,-18.201c0,-7.518 1.603,-13.025 4.809,-16.522c3.207,-3.497 7.999,-5.245 14.377,-5.245Z"
									style="fill-rule:nonzero;"
								></path> <g id="trash"> </g> <g id="vertical-menu"> </g>
								<g id="horizontal-menu"> </g> <g id="sidebar-2"> </g> <g id="Pen"> </g>
								<g id="Pen1" serif:id="Pen"> </g> <g id="clock"> </g> <g id="external-link"> </g>
								<g id="hr"> </g> <g id="info"> </g> <g id="warning"> </g> <g id="plus-circle"> </g>
								<g id="minus-circle"> </g> <g id="vue"> </g> <g id="cog"> </g> <g id="logo"> </g>
								<g id="radio-check"> </g> <g id="eye-slash"> </g> <g id="eye"> </g>
								<g id="toggle-off"> </g> <g id="shredder"> </g>
								<g id="spinner--loading--dots-" serif:id="spinner [loading, dots]"> </g>
								<g id="react"> </g> <g id="check-selected"> </g> <g id="turn-off"> </g>
								<g id="code-block"> </g> <g id="user"> </g> <g id="coffee-bean"> </g>
								<g id="coffee-beans"> <g id="coffee-bean1" serif:id="coffee-bean"> </g> </g>
								<g id="coffee-bean-filled"> </g>
								<g id="coffee-beans-filled"> <g id="coffee-bean2" serif:id="coffee-bean"> </g> </g>
								<g id="clipboard"> </g> <g id="clipboard-paste"> </g> <g id="clipboard-copy"> </g>
								<g id="Layer1"> </g>
							</g>
						</g></svg
					>
				</div>
				<!-- comment  -->
				<p class="text-sm font-light">
					{happyClient.comment}
				</p>
				<div class="flex items-start justify-start space-x-3">
					<!-- avatar -->
					<img
						class="w-12 h-12 rounded-full 2xl:w-12 xl:w-12 lg:w-12 md:w-10 2xl:h-12 xl:h-12 lg:h-12 md:h-10"
						src={happyClient.avatar}
						alt="avatar"
					/>
					<div class="flex flex-col items-start justify-center">
						<!-- name -->
						<p class="text-sm font-bold">
							{happyClient.name}
						</p>
						<!-- bio -->
						<p class="text-sm font-light">
							{happyClient.bio}
						</p>
						<!-- stars -->
						<div>
							<Ratings value={happyClient.stars} max={happyClient.stars}>
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
				</div>
			</div>
		{/each}
	</div>
</div>
