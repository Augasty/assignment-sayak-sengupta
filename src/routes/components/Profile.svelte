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
	<div class="mb-4 ml-40 grid">
		<Avatar.Root class="mr-4 h-28 w-28  ">
			<Avatar.Image
				src={profilepic}
				alt="@shadcn"
				class="border-grey rounded-full border border-4"
			/>
			<Avatar.Fallback class="rounded-full border border-black">KK</Avatar.Fallback>
		</Avatar.Root>
		<div class="flex max-w-28 items-center text-center text-xl font-bold text-gray-700">
			Krishna Kiran
		</div>
	</div>

	<div class="mb-4 ml-8 mr-8 mt-6 grid">
		<div class="flex max-w-lg text-left text-xs text-gray-700">
			Co-Founder and CEO at Duggup - Social network for people in tech. Ex-Amazon Head of
			Engineering. I write hot-takes on building a business, shipping delightful products and
			accelerating product and career growth.
		</div>

		<Button
			variant="outline"
			class="mr-12 max-w-min border border-b-4 border-gray-700 text-xs"
			on:click={toggleFollow}
		>
			{#if isFollowed}
				Followed
			{:else}
				Follow
			{/if}
		</Button>
	</div>

	<div class="mb-0 mb-4 ml-4 mt-6 grid justify-between">
		<div class="justify-start">
			<Avatar.Root class="ml-28">
				<Avatar.Image src={duggup} alt="@shadcn" class="border-grey rounded-full" />
				<Avatar.Fallback class="rounded-full border border-black">DU</Avatar.Fallback>
			</Avatar.Root>
			<div class="ml-24 flex h-min max-w-lg text-right text-sm font-bold text-black">Duggup</div>
			<div class="ml-8 flex h-min max-w-lg text-right text-sm text-xs text-gray-400">
				Co-Founder and CEO
			</div>
		</div>
		<div class="ml-6 flex h-min max-w-lg text-right text-sm text-xs text-black">
			My website <a href="https://www.google.com"
				><SquareArrowOutUpRight size="14" strokeWidth="2" class="ml-1 text-gray-400" /></a
			>
		</div>
	</div>
</section>
