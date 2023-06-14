<template>
    <div>
  
  
      <header class="shadow-sm bg-white">
              
          <nav class="container mx-auto p-4">
            <NuxtLink to="/">Miratech | Sales - Merchant</NuxtLink> 
          </nav>

      </header>
  
      <!-- Output the page content -->

      <div class="container mx-auto p-4">
        <slot />
      </div>
  
    </div>


    <footer class="container mx-auto p-4 flex justify-between border-t-2">
        <ul class="flex gap-4">
                  <li><NuxtLink to="/">Home</NuxtLink></li>
                  <li><NuxtLink to="/about">About</NuxtLink></li>
                  <li><NuxtLink to="/products">Products</NuxtLink></li>
                  <li><NuxtLink to="/cart">Cart</NuxtLink></li>
                  <li><NuxtLink to="/contact">Contact-us</NuxtLink></li>
              </ul>
    </footer>

  </template>


<style>

.router-link-exact-active {
    color: #12b488;
}

</style>