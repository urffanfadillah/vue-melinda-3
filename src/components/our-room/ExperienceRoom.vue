<template>
    <section class="container-fluid blue-theme p-5">
        <div class="cotainer mx-auto row">
            <div class="col-sm-12 mb-5 d-flex align-items-center flex-column">
                <HeadingContent
                    white_title 
                    subTitle="Experience Room"
                    title="Experience Using RS Melinda 2 Room"                    
                />                                    
            </div>
            <div class="col-sm-6 d-flex justify-content-center" v-for="d in data" :key="d.id">
                <div>
                    <HeadingContent
                        white_title 
                        subTitle="RS Melinda 2"
                        :title="d.title"
                        :paragraph="d.content"
                    >
                        <p class="text-white fw-bold">{{d.quote}}</p>
                    </HeadingContent>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
    import HeadingContent from "@/components/utils/HeadingContent.vue"
    export default {
        components: { HeadingContent },
        data() {
            return {
                data: [
                    {
                        id: 1,
                        title: "What Mother Says",
                        content: `“The Best Place and Friendly Nurse”`,
                        quote: `Hannah S. Johnson`
                    },
                    {
                        id: 2,
                        title: "What Mother Says",
                        content: `“The Best Place and Friendly Nurse”`,
                        quote: `Hannah S. Johnson`
                    },                    
                ]
            }
        }
    }
</script>

<style scoped>
    .blue-theme {
        background: #1B4674;
    }
</style>