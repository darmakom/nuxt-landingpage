<script lang="ts" setup>
useSeoMeta({
  titleTemplate: '%s - LANDINGPAGE',
})
</script>

<template>
  <div>
    <NuxtLoadingIndicator color="red" :throttle="0" />
    <NuxtLayout>
      <NuxtPage />
    </NuxtLayout>
  </div>
</template>
