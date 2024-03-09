<script>
	import { Button } from '$lib/components/ui/button';
	import * as Avatar from '$lib/components/ui/avatar';
	import { Home, AlignStartVertical, BookOpen, SquarePlus, ChevronDown } from 'lucide-svelte';
	import profilepic from '../../lib/images/profilepic.jpeg';
	import duggup from '../../lib/images/duggup_logo.jpeg';
</script>

<header class="font-inter flex justify-between mt-2 mr-8 ml-8 border-b border-dashed border-gray-500">
	<div class="flex mb-2">
		<Avatar.Root class="rounded-md mr-2 ml-4 ">
			<Avatar.Image src={duggup} alt="@shadcn"/>
			<Avatar.Fallback class="rounded-full border border-black">DU</Avatar.Fallback>
		</Avatar.Root>

		<div class="flex items-center mr-2 text-md font-bold text-gray-700">
			duggup
		</div>
	</div>
	<div class="flex mb-2">
		<Button variant="ghost" class="mr-4 text-xs"
			><Home size="12" strokeWidth="1" class="mr-2" /> Home</Button
		>

		<Button variant="ghost" class="mr-4 text-xs"
			><AlignStartVertical size="12" strokeWidth="1" class="mr-2" /> Explore</Button
		>

		<Button variant="ghost" class="mr-4 text-xs"
			><BookOpen size="12" strokeWidth="1" class="mr-2" /> Learn</Button
		>

		<Button variant="outline" class="mr-12 border border-b-4 border-gray-700 text-xs"
			><SquarePlus size="12" strokeWidth="1" class="mr-2" /> Post</Button
		>

		<Avatar.Root class="mr-4">
			<Avatar.Image src={profilepic} alt="@shadcn" class="rounded-full border border-black" />
			<Avatar.Fallback class="rounded-full border border-black">KK</Avatar.Fallback>
		</Avatar.Root>
		<div class="flex items-center text-md mr-2 text-gray-700">
			Krishna Kiran <ChevronDown size="16" strokeWidth="1" class="ml-2" />
		</div>
	</div>
</header>
