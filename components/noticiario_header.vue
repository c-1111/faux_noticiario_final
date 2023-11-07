<template>
    <div class="header flex max-[800px]:max-w-[800px] max-[800px]:flex-col max-[800px]:pt-6 max-[800px]:pb-6">
        <div class="logo_holder w-full flex justify-center py-4 font-sf">
            <img src="/img/logo_faux_home.svg" alt="">
        </div>
    </div>
</template>

<script setup>
</script>

<style lang="sass">
.header
    @apply w-full border-b border-black
    .logo_holder
        @apply w-full flex justify-center py-8 font-sf
        img
            @apply w-[80px]
</style>