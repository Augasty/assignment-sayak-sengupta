<!-- CustomCard.svelte -->
<script>
// @ts-nocheck

     export let imageSrc1;
     export let imageSrc2;

     export let text1;
     export let text2;

     
	import { Circle } from 'lucide-svelte';
    import CustomCard from './CustomCard.svelte';
  </script>
  

  <div class="relative mb-24 flex items-center">
    <div class=" -ml-1 mt-4 flex h-max w-max bg-white">
        <Circle size="10" strokeWidth="5" color="#0066FF" />
    </div>
    <div class="flex">
        <CustomCard
            imageSrc={imageSrc1}
            text={text1}
        />

        <CustomCard
            imageSrc={imageSrc2}
            text={text2}
        />
    </div>

    <div class="absolute -ml-20 mt-4 text-xs text-gray-400">Dec 2023</div>
</div>
