<template>
    <section class="flex gap-10">
        <div class="space-y-[10px] w-[50%]">
            <div class="space-y-[5px]">
                <p class="text-[#175CD3] text-[18px]">Support</p>
                <h4 class="text-gray-800 text-[48px] font-semibold">FAQS</h4>
            </div>
            <P class="text-gray-500 text-[24px]">Everything you need to know about the product and billing. Can’t find the answer you’re looking for? Please chat to our friendly team.</P>
        </div>

        <div class="w-[50%] space-y-4">
            <div class="flex justify-between p-4 border-b border-gray-200 rounded-[16px]" v-for="(faq, index) in faqs" :key.id="index" :class="index === 0 ? 'bg-[#F9FAFB] border border-gray-200' : ''">
                <div class="space-y-4">
                    <h3 class="font-semibold">{{ faq.heading }}</h3>
                    <p class="text-sm" :class="faq.showFaq ? 'block' : 'hidden'">{{ faq.content }}</p>
                </div>
                <div  @click="toggleVisibility(faq)">
                    <svg v-if="!faq.showFaq" width="22" height="22" viewBox="0 0 22 22" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M11 7V15M7 11H15M21 11C21 16.5228 16.5228 21 11 21C5.47715 21 1 16.5228 1 11C1 5.47715 5.47715 1 11 1C16.5228 1 21 5.47715 21 11Z" stroke="#98A2B3" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/></svg>
                    <svg v-else width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M8 12H16M22 12C22 17.5228 17.5228 22 12 22C6.47715 22 2 17.5228 2 12C2 6.47715 6.47715 2 12 2C17.5228 2 22 6.47715 22 12Z" stroke="#98A2B3" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/></svg>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
    import { defineComponent } from 'vue';
    export default defineComponent({
      data(){
        return{
            showFaq: true,
            faqs: [
                {
                    heading: 'How many participants can join a ClearLink video conference?',
                    content: 'ClearLink offers flexible meeting options. Depending on your subscription plan, you can host meetings with varying numbers of participants. Our plans are designed to accommodate small team collaborations and large-scale webinars, ensuring you have the right fit for your needs.'
                },
                {
                    heading: 'Can I use ClearLink on multiple devices?',
                    content: 'ClearLink offers flexible meeting options. Depending on your subscription plan, you can host meetings with varying numbers of participants. Our plans are designed to accommodate small team collaborations and large-scale webinars, ensuring you have the right fit for your needs.'
                },
                {
                    heading: 'Is ClearLink compatible with other video conferencing platforms?',
                    content: 'ClearLink offers flexible meeting options. Depending on your subscription plan, you can host meetings with varying numbers of participants. Our plans are designed to accommodate small team collaborations and large-scale webinars, ensuring you have the right fit for your needs.'
                },
                {
                    heading: 'How does ClearLink ensure the security of my video conferences?',
                    content: 'ClearLink offers flexible meeting options. Depending on your subscription plan, you can host meetings with varying numbers of participants. Our plans are designed to accommodate small team collaborations and large-scale webinars, ensuring you have the right fit for your needs.'
                },
                {
                    heading: 'Do I need to download any software to use ClearLink?',
                    content: 'ClearLink offers flexible meeting options. Depending on your subscription plan, you can host meetings with varying numbers of participants. Our plans are designed to accommodate small team collaborations and large-scale webinars, ensuring you have the right fit for your needs.'
                },
                {
                    heading: 'What kind of customer support does ClearLink provide?',
                    content: 'ClearLink offers flexible meeting options. Depending on your subscription plan, you can host meetings with varying numbers of participants. Our plans are designed to accommodate small team collaborations and large-scale webinars, ensuring you have the right fit for your needs.'
                }
            ]
        }
      },
      methods:{
        toggleVisibility(faq){
            faq.showFaq = !faq.showFaq
        }
      }  
    })
</script>

<style scoped>

</style>