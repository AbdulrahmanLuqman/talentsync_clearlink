<template>
    <section class="flex">
        <div class="space-y-[40px] w-[40%]">
            <h3 class="font-semibold text-[38px]">Ready to clear the path to perfect communication?</h3>
            <div class="space-y-[18px]">
                <div v-for="trial in trials" class="flex gap-2 items-center">
                    <svg width="28" height="29" viewBox="0 0 28 29" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M8.75 14.4999L12.25 17.9999L19.25 10.9999M25.6667 14.4999C25.6667 20.9432 20.4433 26.1666 14 26.1666C7.55668 26.1666 2.33334 20.9432 2.33334 14.4999C2.33334 8.0566 7.55668 2.83325 14 2.83325C20.4433 2.83325 25.6667 8.0566 25.6667 14.4999Z" stroke="#175CD3" stroke-width="2.33333" stroke-linecap="round" stroke-linejoin="round"/></svg>
                    <p class="text-[20px] text-gray-600">{{ trial.content }}</p>
                </div>
            </div>
            <div class="space-x-4">
                <button class="border border-gray-400 py-[14px] px-[24px] rounded-[100px] font-semibold hover:bg-gray-400">Talk to sales</button>
                <button class="bg-blue-700 hover:bg-blue-600 py-[14px] px-[24px] rounded-[100px] font-semibold text-white">Start your free trial</button>
            </div>
        </div>
        <div class="absolute right-0">
            <img class="w-[650px]" src="../assets/images/trials-image.png" alt="">
        </div>
    </section>
</template>

<script>
    export default {
        data(){
            return{
                trials: [
                    {
                        content: '30 days free trial'
                    },
                    {
                        content: 'Cancel at any time'
                    },
                    {
                        content: 'Access to all features'
                    },
                    {
                        content: 'Peronalized onboarding'
                    }
                ]
            }
        }
    }
</script>

<style scoped>

</style>