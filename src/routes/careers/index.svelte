<FeaturedImage imageUrl="'/featured-careers.webp'" pageName="Careers" pageTagline="Hiring Experts" imagePosition="center"></FeaturedImage>

<div class="w-screen flex justify-center">
  <div class="w-full max-w-ninety lg:max-w-screen-lg py-8">
    <h3>Currently Hiring for:</h3>
    <div>
      {#each careers as career}
      <div class="flex">
        <div class="flex-grow">
          <h4>{ career.title}</h4>
          <p>{@html career.description}</p>
          <b>{ career.rate }</b>
        </div>
        <div class="flex-shrink align-center">
          <a href="/apply" class="bg-blue text-white text-center p-3 font-semibold hover:bg-blue-transparent">Apply</a>
        </div>
      </div>
      {/each}
    </div>
  </div>
</div>

<SvelteSEO
  title="{ careersSeo.title }"
  description="{ careersSeo.description }"
></SvelteSEO>

<script context="module">
  export const prerender = true
</script>
<script>
  import FeaturedImage from '$lib/featuredImage.svelte'
  import SvelteSEO from 'svelte-seo'
  import { careers as careersSeo } from '../../seo.js'

  const careers = [
    {
      title: 'Welder/Fabricator (Aluminum)',
      description: '<p>Assists our Feed Body Builds and Feed Body Repairs Department.</p>',
      rate: '$15.00 - $25.00',
    }
  ]
</script>