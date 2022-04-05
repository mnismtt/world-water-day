<script></script>

<section class="relative h-screen py-40">
	<img
		src="/images/left_graphic.png"
		alt="Left Graphic"
		class="absolute bottom-0 left-0 w-full lg:w-fit lg:h-1/2"
	/>
	<img
		src="/images/right_graphic.png"
		alt="Right Graphic"
		class="hidden lg:block absolute right-0 top-0 2xl:w-fit h-[95%] w-[50%]"
	/>
	<img src="/images/crab.png" alt="Crab" class="absolute left-0 hidden xl:block top-1/4" />
	<div class="flex h-full px-8 mx-auto lg:max-w-6xl">
		<div class="z-10 flex flex-col justify-center h-full lg:w-1/2">
			<h1 class="headline">Protect Our Water Buddies</h1>
			<p class="font-medium text-lg sm:text-3xl md:text-[20px] leading-[171.5%] mt-6">
				You did not inherit the Earth’s water from your ancestors, you owe it to your future
				generations ahead.
			</p>
			<div class="flex space-x-[27px] mt-14">
				<button class="btn btn-gradient">Let's begin</button>
				<button class="flex items-center space-x-3 btn btn-outline">
					<img src="/images/video_icon.svg" width={32} height={32} alt="Video Icon" />
					<span>Watch video</span>
				</button>
			</div>
		</div>
	</div>
</section>

<style lang="postcss">
	.headline {
		@apply font-bold text-3xl sm:text-4xl md:text-5xl xl:text-[56px];
		line-height: 129%;
		background: linear-gradient(180deg, #1b18f9 0%, #1b18f9 46.35%, #e146ad 100%);
		-webkit-background-clip: text;
		-webkit-text-fill-color: transparent;
		background-clip: text;
		text-fill-color: transparent;
	}

	.btn {
		@apply px-9 py-4 font-semibold md:text-lg lg:text-2xl transition duration-300 hover:opacity-75;
		border-radius: 18px;
	}

	.btn-outline {
		background: linear-gradient(180deg, #1b18f9 0%, #1b18f9 46.35%, #e146ad 100%);
		-webkit-background-clip: text;
		-webkit-text-fill-color: transparent;
		background-clip: text;
		text-fill-color: transparent;
	}

	.btn-gradient {
		@apply text-white;
		background: radial-gradient(255.8% 457.4% at 88.45% 24.64%, #c27fcf 0%, #0368ff 100%)
			/* warning: gradient uses a rotation that is not supported by CSS and may not behave as expected */;
	}
</style>
