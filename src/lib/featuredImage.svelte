<script>
  export let imageUrl
  export let pageName
  export let pageTagline
</script>

<div class="w-screen flex flex-col justify-center items-center bg-center" style="background-image: url({imageUrl}); aspect-ratio: 16/5">
  <div class="w-full max-w-screen-lg bg-gray-600 bg-opacity-40 text-center py-12">
    {#if $$slots.default}
      <slot></slot>
    {:else}
      <h1 class="text-white">{ pageName }</h1>
      <h2 class="text-white">{ pageTagline }</h2>
    {/if}
    
  </div>
</div>