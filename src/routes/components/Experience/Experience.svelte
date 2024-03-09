<script>
	import { Circle, ChevronUp } from 'lucide-svelte';
	import stevejobs from '../../../lib/images/steve-jobs.jpeg';
	import samaltman from '../../../lib/images/samaltman.jpeg';
	import CustomCard from './CustomCard.svelte';
	import * as Avatar from '$lib/components/ui/avatar';

	import duggup from '../../../lib/images/duggup_logo.jpeg';
</script>

<section class="font-inter ml-52 mt-8">
	<div class="relative">
		<!-- vertical line -->
		<div class="absolute bottom-0 left-0 top-0 border-l-2 border-dashed border-gray-400"></div>

		<!-- timeline entries -->
		<div class="relative mb-24 flex items-center">
			<div class="absolute left-0 -ml-1 mt-4 flex h-max w-max bg-white">
				<Circle size="10" strokeWidth="5" color="#0066FF" />
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

			<div class="absolute -ml-20 mt-4 text-xs text-gray-400">Dec 2023</div>
		</div>

		<div class="relative mb-4 flex items-center">

			<div class="absolute left-0 -ml-2 -mt-32 flex h-min w-max">
				<ChevronUp size="17" strokeWidth="2" color="grey" />
			</div>
			<div class="absolute left-0 -ml-2 mt-4 flex h-max w-max bg-white">
				<Circle size="16" strokeWidth="5" color="#0066FF" />
			</div>

			<div class="absolute -ml-36 -mt-4">
				<div class="grid justify-items-end">
					<Avatar.Root class="ml-3">
						<Avatar.Image src={duggup} alt="@shadcn" class="border-grey rounded-full" />
						<Avatar.Fallback class="rounded-full border border-black">DU</Avatar.Fallback>
					</Avatar.Root>
					<div class="text-right text-sm font-bold text-black">Duggup</div>
					<div class="text-[11px] text-gray-400">San Francisco Bay Area</div>
					<div class="text-[11px] text-gray-400">Joined</div>
					<div class="text-[11px] text-gray-400">Nov 2023</div>
				</div>
			</div>
			<div class="absolute ml-12">
				<div class="text-md font-bold text-black">Co-Founder and CEO</div>
				<div class="flex h-min max-w-lg text-[9px] text-gray-400">Full-time · Remote</div>
			</div>
		</div>
	</div>
</section>
