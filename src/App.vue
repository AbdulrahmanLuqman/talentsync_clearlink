<script>
import { defineComponent } from 'vue';
import Navbar from './components/Navbar.vue';
import BackgroundPattern from './components/BackgroundPattern.vue'
import FirstSection from './components/FirstSection.vue'
import Companies from './components/Companies.vue'
import WhyChoose from './components/WhyChoose.vue';
import Testimonials from './components/Testimonials.vue'

export default defineComponent({
    components:{
    Navbar, 
    BackgroundPattern, 
    FirstSection, 
    Companies,
    WhyChoose,
    Testimonials
}
})
</script>

<template>
    <main class="pt-[40px] pb-[96px] space-y-[120px] max-w-[1440px] mx-auto">
        <Navbar class="z-[999] relative mx-[100px]"/>
        <BackgroundPattern class="absolute top-0 left-0 z-[-10]"/>
        <FirstSection class="px-[100px]"/>
        <Companies class="px-[100px]"/>
        <WhyChoose class="px-[100px]"/>
        <Testimonials class="px-[100px]"/>
    </main>
</template>

<style scoped>

</style>
