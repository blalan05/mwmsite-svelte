<div class="w-screen bg-blue-800 px-8">
  <div class="w-full grid grid-cols-2 lg:grid-cols-4 gap-8 text-white">
    {#each services as service}
    <div>
      <img src="{service.image}" alt="" />
      <h4 class="text-2xl">{ service.title }</h4>
      <p>{ service.content }</p>
    </div>
    {/each}
  </div>
</div>

<script>
  const services = [
    {
      title: 'Custom Fabrication',
      content: 'We make custom stuff, and we fabricate it. Thus why we call this custom fabrication.',
      image: '/service-fabrication.webp'
    },
    {
      title: 'Industry Vendors',
      content: 'We work with many of the commerical retailers. Availability and Savings we can pass on to you.',
      image: '/service-venders.webp'
    },
    {
      title: 'Hiring Experts',
      content: 'Looking for a job? We are looking fo motivated, skilled and safe-minded industry leaders',
      image: '/service-experts.webp'
    },
    {
      title: 'MWM Promise',
      content: 'We will always do the best we can to create a solution to your problem.',
      image: '/service-promise.webp'
    }
  ]

</script>
