<script>
    import { Card, Button} from 'flowbite-svelte';
    export let img = "";
    export let title = "";
    export let uniDegree = "";
    export let description = "";
    export let stats = "";
</script>

  
  <div class="flex flex-col items-center bg-white shadow-lg rounded-lg overflow-hidden w-500 h-50 object-fill"> <!-- Adjust width and height as needed -->
    <img src={img} class="aspect-square object-cover" alt="{title}" />
    <div class="p-4 flex flex-col h-full">
      <h5 class="text-xl font-bold text-gray-900 dark:text-white mb-2">{title}</h5>
      <p class="text-gray-700 dark:text-gray-400 mb-3 flex-grow">{uniDegree}</p>
      <p class="text-gray-700 dark:text-gray-400 mb-3">{stats}</p>
      <Button>Send message</Button>
    </div>
  </div>