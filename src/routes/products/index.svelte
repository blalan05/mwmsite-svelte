<div class="w-screen flex justify-center">
  <div class="w-full max-w-screen-lg">
    <h2>Products</h2>
    <div class="grid grid-cols-3">
      {#each products as product}
        <div><a href="{ product.link }">{ product.title }</a></div>
      {/each}
    </div>
  </div>
</div>

<script>
  const products = [
    {
      title: 'Feed Bodies',
      link: '',
      content: '',
      image: '',
    },
    {
      title: 'Conveyors',
      link: '',
      content: '',
      image: '',
    },
    {
      title: 'Distributors',
      link: '',
      content: '',
      image: '',
    },
    {
      title: 'Elevator Legs',
      link: '',
      content: '',
      image: '',
    },
    {
      title: 'Mixers',
      link: '',
      content: '',
      image: '',
    },
    {
      title: 'Manwalks/Catwalks',
      link: '',
      content: '',
      image: '',
    },
    {
      title: 'Towers',
      link: '',
      content: '',
      image: '',
    },
    {
      title: 'Two Ways',
      link: '',
      content: '',
      image: '',
    },
  ]

</script>