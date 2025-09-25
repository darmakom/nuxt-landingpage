<script setup lang="ts">
    const menus = ref([
        { label: 'Home', to: '/' },
        { label: 'About', to: '/about' },
        { label: 'Contact', to: '/contact' },
    ])
</script>

<template>
    <div class="bg-gray-100 text-gray-800 dark:bg-gray-950 dark:text-gray-100 min-h-screen flex flex-col">
        <header class="sticky top-0 bg-gray-50/70 border-b border-gray-500/50 h-[68px] flex">
            <PageContainer class="flex-1 flex items-center justify-between">
                <NuxtLink to="/" class="font-bold text-lg">LANDING PAGE</NuxtLink>
                <div>
                    <nav class="flex gap-4">
                        <ul v-for="menu in menus">
                            <li>
                                <NuxtLink :to="menu.to" class="hover:text-primary-500">{{ menu.label }}</NuxtLink>
                            </li>
                        </ul>
                    </nav>
                </div>
            </PageContainer>
        </header>
        <main class="flex-1">
            <slot />
        </main>
        <footer class="border-t border-gray-500/50 h-[48px] flex">
            <PageContainer class="flex-1 flex items-center justify-between">
                <div class="text-sm flex-1">
                    &copy; 2025
                </div>
                <div class="flex gap-1">
                    <Icon name="material-symbols:favorite-outline" class="text-lg text-primary-500" />
                    <Icon name="uil:instagram" class="text-lg text-primary-500" />
                </div>
            </PageContainer>
        </footer>
    </div>
</template>