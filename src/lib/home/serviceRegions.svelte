<div class="w-screen bg-gray-200 py-8">
  <div class="w-full max-w-screen-lg grid grid-cols-1 md:grid-cols-2 mx-auto">
    <div>
      <h2 class="text-4xl text-blue-800 font-semibold mb-4">MWM Service Regions</h2>
      <ul class="text-2xl leading-relaxed">
        {#each regions as region}
        <li class="uppercase">{ region }</li>
        {/each}
      </ul>
    </div>
    <div>
      <img src="/service-regions.png" alt="MWM Services the greater Midwest of North America" />
    </div>
  </div>
</div>

<script>
  const regions = ['Wisconsin', 'Minnesota', 'Illinois', 'Indiana', 'and More']
</script>