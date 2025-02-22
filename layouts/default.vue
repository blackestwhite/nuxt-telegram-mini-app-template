<script setup>
useHead({
    script: [
        {
            src: '/telegram-web-app.js',
            defer: true
        }
    ]
})
</script>
<template>
    <div>
        <main>
            <ClientOnly>
                <slot />
            </ClientOnly>
        </main>
    </div>
</template>