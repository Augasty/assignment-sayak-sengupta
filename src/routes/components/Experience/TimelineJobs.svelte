<!-- CustomCard.svelte -->
<script>
	// @ts-nocheck

	export let icon, company, address, joiningDate, role, jobtype;

	import * as Avatar from '$lib/components/ui/avatar';
	import { ChevronUp, CircleDot } from 'lucide-svelte';
</script>

<div class="relative mb-24 flex items-center">
	<div class="-ml-2 -mt-36 h-min w-max bg-white">
		<ChevronUp size="17" strokeWidth="2" color="grey" />
	</div>
	<CircleDot
		class="absolute left-0 -ml-5 -mt-6"
		size="40"
		strokeWidth="4"
		color="#fff"
		fill="#0066FF"
	/>

	<div class="absolute -ml-36 -mt-4">
		<div class="grid justify-items-end">
			<Avatar.Root class="ml-3">
				<Avatar.Image src={icon} alt="@shadcn" class="border-grey rounded-full" />
				<Avatar.Fallback class="rounded-full border border-black">DU</Avatar.Fallback>
			</Avatar.Root>
			<div class="text-right text-sm font-bold text-black">{company}</div>
			<div class="text-[11px] text-gray-400">{address}</div>
			<div class="text-[11px] text-gray-400">Joined</div>
			<div class="text-[11px] text-gray-400">{joiningDate}</div>
		</div>
	</div>
	<div class="absolute ml-12">
		<div class="text-md font-bold text-black">{role}</div>
		<div class="flex h-min max-w-lg text-[9px] text-gray-400">{jobtype}</div>
	</div>
</div>
