<div class="w-screen flex justify-center py-8">
  <div class="w-full max-w-ninety lg:max-w-screen-lg">
    {#each services as service}
    <a href="{ service.link }" class="block">
      <div class="mt-8 py-20 bg-blue text-white bg-center bg-no-repeat bg-cover" style="background-image: url({ service.image })">
        <h3 class="pl-5">{ service.title }</h3>
      </div>
    </a>
    <p>{ service.content }</p>
    {/each}
  </div>
</div>

<script>
  const services = [
    {title: 'Feed Body Repairs', link: '/services/feed-body-repairs', content: '', image: '/services/services-feed-body-repairs.webp'},
    {title: 'Manufacturing', link: '/services/manufacturing', content: '', image: '/services/services-manufacturing.webp'},
    {title: 'Road Crew/Millwrights', link: '/services/road', content: '', image: '/services/services-millwright.webp'},
    {title: 'Machine Shop', link: '/services/machine-shop', content: '', image: '/services/services-machining.webp'},
    {title: 'Waterjet Cutting', link: '/services/waterjet', content: ''},
    {title: 'Drafting', link: '/services/drafting', content: ''},
    {title: 'Sandblasting', link: '/services/sandblasting', content: ''},
    {title: 'Painting', link: '/services/painting', content: ''},
    {title: 'Hot-dipped Steel', link: '/services/hot-dipped-steel', content: ''},
    {title: 'Truck Repairs', link: '/services/truck-repairs', content: ''},
    {title: 'Buy Parts/Materials', link: '/services/parts', content: ''},
    {title: 'Advising/Consulting', link: '/services/consulting', content: ''}
  ]
</script>