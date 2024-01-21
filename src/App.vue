<script>
import { defineComponent } from 'vue';
import Navbar from './components/Navbar.vue';
import BackgroundPattern from './components/BackgroundPattern.vue'
import FirstSection from './components/FirstSection.vue'

export default defineComponent({
    components:{
        Navbar, BackgroundPattern, FirstSection
    }
})
</script>

<template>
    <main class="pt-[40px] px-[100px] pb-[96px] space-y-[120px]">
        <Navbar class="z-[999] relative"/>
        <BackgroundPattern class="absolute top-0 left-0 z-[-10]"/>
        <FirstSection />
    </main>
</template>

<style scoped>

</style>
