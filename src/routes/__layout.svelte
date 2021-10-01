<nav class="h-20 w-screen bg-gray-800 flex justify-center">
  <ul class="flex w-full max-w-screen-lg items-center">
    <li class="inline-block h-full">
      <a href="/" class="inline-block h-5/6 pt-4">
        <img src="/logo.png" alt="Midwest Welding & Manufacturing Logo" class="h-full">
      </a>
    </li>
    <li class="flex-grow"></li>
    {#each menu_items as item}
    <li class="inline-block h-full text-white hover:bg-gray-200 hover:text-gray-800">
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

<footer class="w-screen h-8 bg-gray-800">
  
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