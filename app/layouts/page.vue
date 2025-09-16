<template>
    <div class="bg-gray-100 text-gray-800 dark:bg-gray-950 dark:text-gray-100 min-h-screen">
        <header class="border-b border-gray-500/50 h-10 flex">
            <PageContainer class="flex-1 flex items-center">
                LANDING PAGE
            </PageContainer>
        </header>
        <main>
            <slot />
        </main>
        <footer>

        </footer>
    </div>
</template>