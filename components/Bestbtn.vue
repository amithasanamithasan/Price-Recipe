<script lang="ts" setup>

defineProps<{
lavel:string;

to:string;
}>();
</script>

<template>
          <NuxtLink :to="to" class="px-4 py-2 text-black self-start bg-amber-600 rounded-md text-base lg:text-lg cursor-pointer">
            <slot>{{ lavel }}</slot>
            </NuxtLink>
</template>


