<script>
	import stevejobs from '../../../lib/images/steve-jobs.jpeg';
	import samaltman from '../../../lib/images/samaltman.jpeg';
	import desktopbg from '../../../lib/images/desktopbg.jpeg';
	import mapplan from '../../../lib/images/mapplan.png';

	import duggup from '../../../lib/images/duggup_logo.jpeg';
	
	import betterup from '../../../lib/images/betterup.jpeg';
	import TimelineCards from './TimelineCards.svelte';
	import TimelineJobs from './TimelineJobs.svelte';
</script>

<section class="font-inter ml-52 mt-8">
	<div class="relative">
		<!-- vertical line -->
		<div class="absolute -bottom-24 left-0 top-0 border-l-2 border-dashed border-gray-400"></div>

		<!-- timeline cards -->
		<TimelineCards
			imageSrc1={stevejobs}
			imageSrc2={samaltman}
			text1={'No amount of technology can convert a bad story into a good story.'}
			text2={"Most people don't have original ideas. Here is how Sam Altman pushes himself to have..."}
		/>

		<!-- timeline jobs -->
		<TimelineJobs
			icon={duggup}
			company={'Duggup'}
			address={'San Francisco Bay Area'}
			joiningDate={'Nov 2023'}
			role={'Co-Founder and CEO'}
			jobtype={'Full-time · Remote'}
		/>

		<!-- timeline cards -->
		<TimelineCards
			imageSrc1={desktopbg}
			imageSrc2={mapplan}
			text1={'Startup Lesson I am reflecting. Don\'t build for the "average person".'}
			text2={'Your biggest regrets at 80 will be acts of omission.'}
		/>


				<!-- timeline jobs -->
				<TimelineJobs
				icon={betterup}
				company={'BetterUp'}
				address={'San Francisco Bay Area'}
				joiningDate={'Sep 2022'}
				role={'VP Engineering'}
				jobtype={'Full-time'}
			/>
	
	</div>
</section>
