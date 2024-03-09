<script>
	import { Button } from '$lib/components/ui/button';
	import * as Avatar from '$lib/components/ui/avatar';
	import { SquareArrowOutUpRight } from 'lucide-svelte';
	import profilepic from '../../lib/images/profilepic.jpeg';
	import duggup from '../../lib/images/duggup_logo.jpeg';

	let isFollowed = false;

	function toggleFollow() {
		isFollowed = !isFollowed;
	}
</script>

<section class="font-inter mt-8 flex">
 <div class="ml-20 border-l border-dashed border-gray-500">s</div>
</section>
