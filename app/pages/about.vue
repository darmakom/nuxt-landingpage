<script lang="ts" setup>
    definePageMeta({
       layout: 'page'   
    })

    useSeoMeta({
        title: 'About'
    })
</script>

<template>
    <section class="h-96 bg-gray-200">
        <PageContainer>
            <div class="text-primary-500 text-2xl font-bold">
                About Page
            </div>
            <img src="assets/images/samantha-borges-gXsJ9Ywb5as-unsplash.jpg" class="mt-6 w-[300px]" />
        </PageContainer>
    </section>
    <section class="h-[1000px] bg-gray-300">
        <PageContainer>
            <div class="text-primary-500 text-2xl font-bold">
                Section baru
            </div>
        </PageContainer>
    </section>

</template>