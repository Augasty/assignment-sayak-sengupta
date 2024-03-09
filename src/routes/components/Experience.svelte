<script>
	import { Circle } from 'lucide-svelte';
	import stevejobs from '../../lib/images/steve-jobs.jpeg';
	import samaltman from '../../lib/images/samaltman.jpeg';
	import CustomCard from './CustomCard.svelte';
</script>

<section class="font-inter ml-20 mt-8">
	<div class="relative">
		<!-- vertical line -->
		<div class="absolute bottom-0 left-0 top-0 border-l-2 border-dashed border-gray-400"></div>

		<div class="relative mb-4 flex items-center">
			<div
				class="absolute left-0 -ml-3 mt-4 flex h-6 w-6 items-center justify-center rounded-full bg-blue-500"
			>
				<Circle />
			</div>
			<div class="flex">
				<CustomCard
					imageSrc={stevejobs}
					text={'No amount of technology can convert a bad story into a good story.'}
				/>

				<CustomCard
					imageSrc={samaltman}
					text={"Most people don't have original ideas. Here is how Sam Altman pushes himself to have..."}
				/>
			</div>

			<div class="absolute -ml-12 mt-4">date</div>
		</div>

		<div class="relative mb-4">
			<div
				class="absolute left-0 -ml-3 mt-1 flex h-6 w-6 items-center justify-center rounded-full bg-blue-500"
			>
				<Circle />
			</div>
		</div>

		<div class="relative mb-4">
			<div
				class="absolute left-0 -ml-3 mt-1 flex h-6 w-6 items-center justify-center rounded-full bg-blue-500"
			>
				<Circle />
			</div>
			<div class="ml-8">
				<p>
					Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia Curae;
					Donec nec justo.
				</p>
			</div>
		</div>
	</div>
</section>
