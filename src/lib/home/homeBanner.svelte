<div class="w-screen home_banner">
  <div class="w-full py-10">
    <div class="bg-blue-800 bg-opacity-40 py-8 flex justify-center flex-col">
      <h1 class="text-7xl text-white font-extrabold uppercase text-shadow text-center leading-relaxed">Midwest Welding & Manufacturing</h1>
      <h2 class="text-4xl text-white font-extrabold uppercase text-shadow text-center leading-normal">Repairing Your Past...Fabricating Your Future</h2>
      <div class="text-center">
        <a href="/" class="inline-block mt-3 rounded bg-white py-3 px-5 text-xl hover:text-white hover:bg-transparent border-solid border-2 border-white">Tell Us About Your Project</a>
      </div>
    </div>
    <div class="mt-8 max-w-screen-lg w-full mx-auto">
      <hr />
      <div class="grid grid-cols-3 gap-4 mt-5">
        {#each FeaturedServices as service}
          <div class="text-white bg-red-800 bg-opacity-70 p-5 my-5">
            <h3 class="text-">{ service.title }</h3>
            <p>{ service.content }</p>
          </div>
        {/each}
      </div>
    </div>
  </div>
</div>

<style>
  .home_banner {
    background-image: url('/home_banner.webp');
  }
</style>

<script>
  const FeaturedServices = [
    {title: 'Field Service', content: 'Whether a difficult repair or equipment installation, our teams are ready for the job.'},
    {title: 'Shop Services', content: 'Tools and Fabrication ready to accomplish simple or complex jobs.'},
    {title: 'Feed Body Services', content: 'Our custom made-to-order Bulk Feed Body Trucks or Semis are perfectly engineered.'}
  ]

</script>