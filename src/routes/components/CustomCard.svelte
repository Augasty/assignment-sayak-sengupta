<!-- CustomCard.svelte -->
<script>
    /**
	 * @type {any}
	 */
     export let imageSrc;
    /**
	 * @type {any}
	 */
     export let text;

    import * as Card from '$lib/components/ui/card/index.js';
	import * as Avatar from '$lib/components/ui/avatar';
  </script>
  
  <Card.Root class="ml-8 h-[180px] w-[280px]">
    <Avatar.Root
      class="ml-0 mr-0 h-[120px] w-[280px] rounded-bl-none rounded-br-none rounded-tl-sm rounded-tr-sm"
    >
      <Avatar.Image src={imageSrc} alt="@shadcn" class="h-full w-full object-cover" />
      <Avatar.Fallback class="rounded-full">SJ</Avatar.Fallback>
    </Avatar.Root>
    <div class="mt-3 mb-3 ml-4 mr-4 flex max-w-lg text-left text-xs text-gray-700">
        {text}
    </div>
  </Card.Root>