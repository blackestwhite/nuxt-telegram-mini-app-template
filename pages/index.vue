<script setup>
const { MainButton, useWebAppPopup, useWebApp } = await import('vue-tg')

const { showAlert } = useWebAppPopup()

const { initDataUnsafe } = useWebApp()
</script>
<template>
    <section>
        Hello Telegram Mini App

        <h2>
            Your name is {{ initDataUnsafe.user?.first_name }}
        </h2>

        <MainButton @click="() => showAlert('Hi')" text="show alert"/>
    </section>
</template>