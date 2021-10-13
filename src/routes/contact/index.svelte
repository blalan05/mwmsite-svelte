<FeaturedImage imageUrl="'/featured-about.webp'" pageName="Contact Us" pageTagline="Looking Forward to Hearing from You"></FeaturedImage>

<div class="w-screen flex justify-center bg-blue py-8">
  <form method="post" name="contactUs" data-netlify="true" class="w-full max-w-ninety lg:max-w-screen-lg grid grid-cols-2">
      <div class="m-3"><input class="w-full" bind:value="{name}" type="text" placeholder="Name" /></div>
      <div class="m-3"><input class="w-full" bind:value="{email}" type="text" placeholder="Email" /></div>
      <div class="col-span-2 m-3">
        <p class="text-white">Message: </p>
        <textarea class="w-full" bind:value="{message}" rows="5" />
      </div>
      <div class="col-span-2 text-right">
        <button on:click="{handleSubmit}" class="border-2 border-blue-400 text-blue-400 mr-3 py-2 px-5 rounded-sm font-semibold text-xl">Submit</button>
      </div>
    </form>
</div>

<div class="w-screen flex justify-center bg-white my-8">
  <div class="w-full max-w-screen-lg">
    <iframe title="MWM Main Office and shops" src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2903.5443209820833!2d-88.84660488422072!3d43.30286358303125!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x880683153e7957d7%3A0x8d71b0f8462b3eb4!2s202%20Harrison%20St%2C%20Reeseville%2C%20WI%2053579!5e0!3m2!1sen!2sus!4v1633112678297!5m2!1sen!2sus" width="100%" style="border:0; aspect-ratio: 16/9" allowfullscreen loading="lazy"></iframe>
  </div>
</div>

<svelte:head>
  <title>Contact | MWM</title>
  <meta name="description" content="Contact MWM for all your custom made agricultural equipment." />
  <meta
    name="robots"
    content="index, follow, max-snippet:-1, max-image-preview:large, max-video-preview:-1"
  />
</svelte:head>

<script>
  let name
  let email
  let message

  import FeaturedImage from '$lib/featuredImage.svelte'
  function encode(data) {
    return Object.keys(data)
      .map(key => encodeURIComponent(key) + "=" + encodeURIComponent(data[key]))
      .join("&")
  }

  const handleSubmit = (event) => {
    event.preventDefault()
    fetch("/contact", {
      method: "POST",
      headers: { "Content-Type": "application/x-www-form-urlencoded" },
      body: encode({
        'form-name': 'contactUs',
        'name': name,
        'email': email,
        'message': message
      })
    }).then(() => console.log("Success"))
  }
</script>
