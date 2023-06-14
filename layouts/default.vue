<template>
    <div>
  
  
      <header id="nav" class="shadow-lg bg-white">
          <nav class="container-fluid mx-auto p-4 flex justify-between">
              <NuxtLink to="/" class="font-bold">Miratech | Sales</NuxtLink>
              <ul class="flex gap-4">
                  <li><NuxtLink to="/">Home</NuxtLink></li>
                  <li><NuxtLink to="/about">About</NuxtLink></li>
                  <li><NuxtLink to="/products" class="btn">Products</NuxtLink></li>
                  <li><NuxtLink to="/cart">Cart</NuxtLink></li>
                  <li><NuxtLink to="/contact">Contact-us</NuxtLink></li>
              </ul>
          </nav>
      </header>
  
      <!-- Output the page content -->

      <div class="container mx-auto p-4">
        <slot />
      </div>
  
    </div>
  </template>


<style>

#nav{
  border-radius: 10px;
}

.router-link-exact-active {
    color: #12b488;
}

</style>