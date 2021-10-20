<script context="module">
  export const prerender = true
</script>
<script>
  import HomeBanner from '$lib/home/homeBanner.svelte'
  import QuickContact from '$lib/home/homeQuickContact.svelte'
  import ServiceHighlights from '$lib/home/serviceHighligt.svelte'
  import ServiceRegions from '$lib/home/serviceRegions.svelte'
</script>

<HomeBanner />
<QuickContact />
<ServiceHighlights />
<ServiceRegions />

<svelte:head>
  <title>Home | MWM</title>
  <meta name="description" content="MWM is a custom agricultural equipment manufacturer with 75yrs of providing products and repair services to greater midwest." />
  <meta
    name="robots"
    content="index, follow, max-snippet:-1, max-image-preview:large, max-video-preview:-1"
  />
</svelte:head>
