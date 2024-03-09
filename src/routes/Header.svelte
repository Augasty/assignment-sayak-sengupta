<script>
	import { Button } from '$lib/components/ui/button';
	import * as Avatar from '$lib/components/ui/avatar';
	import { Home, AlignStartVertical, BookOpen, SquarePlus, ChevronDown } from 'lucide-svelte';
	import profilepic from '../lib/images/profilepic.jpeg';
</script>

<header class="font-inter">
	<div class="mt-2 flex">
		<Button variant="ghost" class="mr-4 text-xs"
			><Home size="12" strokeWidth="1" class="mr-2" /> Home</Button
		>

		<Button variant="ghost" class="mr-4 text-xs"
			><AlignStartVertical size="12" strokeWidth="1" class="mr-2" /> Explore</Button
		>

		<Button variant="ghost" class="mr-4 text-xs"
			><BookOpen size="12" strokeWidth="1" class="mr-2" /> Learn</Button
		>

		<Button variant="outline" class="mr-12 border border-b-4 border-black text-xs"
			><SquarePlus size="12" strokeWidth="1" class="mr-2" /> Post</Button
		>

		<Avatar.Root  class="mr-4">
			<Avatar.Image src={profilepic} alt="@shadcn" class="rounded-full border border-black" />
			<Avatar.Fallback class="rounded-full border border-black">KK</Avatar.Fallback>
		</Avatar.Root>
		<div  class="flex items-center">Krishna Kiran <ChevronDown size="16" strokeWidth="1" class="ml-2"/></div>
	</div>
</header>
