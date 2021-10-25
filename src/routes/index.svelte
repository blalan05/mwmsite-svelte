
<HomeBanner />
<QuickContact />
<ServiceHighlights />
<ServiceRegions />

<SvelteSEO 
title="Home | MWM"
description="Midwest Welding & Manufacturing (MWM) is a custom agricultural equipment manufacturer with 75yrs of providing products and repair services to greater midwest."
></SvelteSEO>

<script context="module">
  export const prerender = true
</script>
<script>
  import HomeBanner from '$lib/home/homeBanner.svelte'
  import QuickContact from '$lib/home/homeQuickContact.svelte'
  import ServiceHighlights from '$lib/home/serviceHighligt.svelte'
  import ServiceRegions from '$lib/home/serviceRegions.svelte'
  import SvelteSEO from 'svelte-seo'
</script>
