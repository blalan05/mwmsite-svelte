<div class="w-screen bg-black flex justify-center pt-12 lg:pt-24">
  <div class=" w-full max-w-ninety lg:max-w-screen-lg">
    <h3 class="text-white text-4xl font-semibold">Quick Contact</h3>
    <div class="grid grid-cols-1 lg:grid-cols-3 gap-4">
      {#each contacts as contact}
      <div class="text-white bg-gray-400">
        <h4 class="text-3xl font-semibold">{ contact.title }</h4>
        <p class="text-xl">{ contact.contact }</p>
        <p class="text-xl"><a rel="external" href="tel:{contact.contact}">{contact.phone}</a></p>
        <p class="text-xl"><a rel="external" href="mailto:{contact.email}">{contact.email}</a></p>
      </div>
      {/each}
    </div>
  </div>
</div>

<script>
  const contacts = [
    {
      title: 'Parts Dept',
      contact: 'Ryan Goodhue',
      phone: '920-927-3851',
      email: 'rgoodhue@mgrf.com'
    },
    {
      title: 'Shop Dept',
      contact: 'Ryan Goodhue',
      phone: '920-927-3854',
      email: 'rgoodhue@mgrf.com'
    },
    {
      title: 'Road Dept',
      contact: 'Zoom Neuman',
      phone: '920-988-9446',
      email: 'zneuman@mgrf.com'
    }
  ]
</script>