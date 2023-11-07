<template>
    <div class="header flex max-[800px]:max-w-[800px] max-[800px]:flex-col max-[800px]:pt-6 max-[800px]:pb-6">
        <div class="logo_holder2 w-full flex justify-center py-4 font-sf max-[800px]:hidden">
            
        </div>
        <div class="logo_holder w-full flex justify-center py-4 font-sf">
            <img src="/img/logo_faux_home.svg" alt="">
        </div>
        <div class="logo_holder w-full flex justify-center py-4 font-sf gap-24">
            <a to="/https://faux-site.netlify.app/" class="link pl-32 pt-2 max-[800px]:pl-0">
                <div class="text"> _proyecto faux</div>
            </a>
            <!-- <a to="/" class="link pt-2">
                <div class="text">redes sociales</div>
            </a> -->
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