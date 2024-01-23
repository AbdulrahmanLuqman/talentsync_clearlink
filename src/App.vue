<script>
import { defineComponent } from 'vue';
import Navbar from './components/Navbar.vue';
import BackgroundPattern from './components/BackgroundPattern.vue'
import FirstSection from './components/FirstSection.vue'
import Companies from './components/Companies.vue'
import WhyChoose from './components/WhyChoose.vue';
import Testimonials from './components/Testimonials.vue'
import Faq from './components/Faq.vue'
import Trial from './components/Trial.vue';
import Footer from './components/Footer.vue'

export default defineComponent({
    components:{
    Navbar,
    BackgroundPattern,
    FirstSection,
    Companies,
    WhyChoose,
    Testimonials,
    Faq,
    Trial,
    Footer
}
})
</script>

<template>
    <main class="pt-[40px] flex flex-col gap-[120px] max-w-[1440px] mx-auto">
        <Navbar class="z-[999] relative mx-[100px] max-[1328px]:mx-[50px] max-[1145px]:mx-[10px]"/>
        <BackgroundPattern class="absolute top-0 left-0 z-[-10]"/>
        <FirstSection class="section px-[100px]"/>
        <Companies class="section px-[100px]"/>
        <WhyChoose class="section px-[100px]"/>
        <!-- <Testimonials class="px-[100px]"/>
        <Faq class="px-[100px]"/>
        <Trial class="pl-[100px]"/>
        <Footer class="pt-10"/> -->
    </main>
</template>

<style scoped>
@media (max-width: 1158px){
    main{
        gap: 50px;
    }
}
@media (max-width: 1328px){
    .section{
        padding: 0 50px;
    }
}

@media (max-width: 1145px){
    .section{
        padding: 0 10px;
    }
}
</style>
