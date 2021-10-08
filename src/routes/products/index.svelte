<FeaturedImage imageUrl="'/products/featured-products.webp'" pageName="Products" pageTagline="Custom-made for every need"></FeaturedImage>

<div class="w-screen my-8 flex justify-center">
  <div class="w-full max-w-ninety lg:max-w-screen-lg">
    <div>
      {#each products as product}
        <a href="{ product.link }" class="block">
          <div class="mt-8 py-20 bg-blue text-white bg-center bg-no-repeat bg-cover" style="background-image: url({ product.image })">
            <h3 class="pl-5">{ product.title }</h3>
          </div>
        </a>
        <p>{ product.content }</p>
      {/each}
    </div>
  </div>
</div>

<svelte:head>
  <title>Products | MWM</title>
  <meta name="description" content="MWM has been building custom agricultural equipment for more than 75 years." />
  <meta
    name="robots"
    content="index, follow, max-snippet:-1, max-image-preview:large, max-video-preview:-1"
  />
</svelte:head>

<script>
  import FeaturedImage from '$lib/featuredImage.svelte'

  const products = [
    {
      title: 'Feed Bodies',
      link: '/products/feed-bodies',
      content: 'You can get our custom made to order Feed bodies in variety of lengths, outputs and options.',
      image: '/products/products-feed-body.webp',
    },
    {
      title: 'Conveyors',
      link: '/products/conveyors',
      content: '',
      image: '/products/products-conveyors.webp',
    },
    {
      title: 'Distributors',
      link: '/products/distributors',
      content: '',
      image: '/products/products-distributors.webp',
    },
    {
      title: 'Elevator Legs',
      link: '/products/elevators',
      content: '',
      image: '/products/products-elevators.webp',
    },
    {
      title: 'Mixers',
      link: '/products/mixers',
      content: '',
      image: '/products/products-mixers.webp',
    },
    {
      title: 'Catwalks/Manwalks',
      link: '/products/catwalks',
      content: '',
      image: '/products/products-catwalks.webp',
    },
    // {
    //   title: 'Towers',
    //   link: '',
    //   content: '',
    //   image: '',
    // },
    // {
    //   title: 'Two Ways',
    //   link: '',
    //   content: '',
    //   image: '',
    // },
  ]

</script>