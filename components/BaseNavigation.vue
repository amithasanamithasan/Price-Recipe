<script lang="ts" setup>

</script>

<template>
    <div>
        <header class="py-4 border-b  bg-slate-700 opacity-60 z-10 overflow-auto ">
    <nav class="flex container items-center">
      <NuxtLink to="/" class="flex gap-1 items-center">
        <img class="w-14 " src="/icon-green.png" alt="" />
        <span class="text-3xl font-extrabold ">Nuxtcipes</span>
      </NuxtLink>
      <ul class="flex gap-6 ml-auto text-xl font-bold capitalize">
        <li>
     <NuxtLink to="/">Home</NuxtLink>
        </li>
        <li>
        <NuxtLink to="/about">About</NuxtLink>
        </li>
        <li>
      <NuxtLink to="/contact"> Contact </NuxtLink>
        </li>
        <li>
       <NuxtLink to="/services" >Services</NuxtLink>
        </li>
        <li>
       <NuxtLink to="/login" >Login</NuxtLink>
        </li>
      </ul>
      <slot></slot> 
    </nav>



  </header>
    </div>
</template>

