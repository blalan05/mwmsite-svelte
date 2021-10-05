<nav class="h-16 lg:h-20 w-screen bg-darkGray justify-center flex">
  <ul class="w-full max-w-screen-lg items-center hidden lg:flex">
    <li class="inline-block h-full">
      <a href="/" class="inline-block h-5/6 pt-4">
        <img src="/logo-bw.webp" alt="Midwest Welding & Manufacturing Logo" class="h-full">
      </a>
    </li>
    <li class="flex-grow"></li>
    {#each menu_items as item}
    <li class="inline-block h-full text-white hover:text-opacity-70">
      <a href="{item.route}" class="h-full flex items-center px-3 text-xl">
        <span>{item.text}</span>
      </a>
    </li>
    {/each}
  </ul>
</nav>

<div class="main_content">
  <slot></slot>
</div>

<footer class="w-screen bg-darkGray grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 py-8">
  <div>
    <img src="/logo.png" alt="MWM Logo" class="w-full max-w-sm mx-auto" />
  </div>
  <div class="text-center md:text-left text-white mb-7">
    <h3>Midwest Welding & Manufacturing</h3>
    <p>202 Harrison Street</p>
    <p>P.O. Box 39</p>
    <p>Reeseville, WI 53579</p>
    <p>Phone: (920) 927-3851</p>
    <p>Fax: (920) 927-5551</p>
  </div>
  <div class="text-white text-center mb-7">
    <h3 class="text-center">Why Choose MWM</h3>
    <h4 class="text-center">Custom Fabrication</h4>
    <h4 class="text-center">Industry Vendors</h4>
    <h4 class="text-center">Hiring Experts</h4>
    <h4 class="text-center">MWM Promise</h4>
  </div>
  <div class="text-white text-center">
    <nav>
      <ul>
        <li>About</li>
        <li>Vendors</li>
        <li>Products</li>
        <li>Services</li>
        <li>Contact</li>
      </ul>
    </nav>
  </div>
</footer>

<script>
  import "../styles/tailwind-output.css"

  const menu_items = [
    {text: 'Home', route: '/'},
    {text: 'About', route: '/about'},
    {text: 'Products', route: '/products'},
    {text: 'Vendors', route: '/vendors'},
    {text: 'Contact', route: '/contact'}
  ]
</script>