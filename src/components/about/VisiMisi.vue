<template>
    <section class="container-fluid blue-theme p-5">
        <div class="cotainer mx-auto row">
            <div class="col-sm-6" v-for="d in data" :key="d.id">
                <HeadingContent
                    white_title 
                    subTitle="RS Melinda 2"
                    :title="d.title"
                    :paragraph="d.content"
                />
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
                        title: "Visi Kami",
                        content: `Menjadi Rumah Sakit Umum Terkemuka dengan Unggulan Bedah dan Anak di Indonesia Khususnya Jawa Barat`
                    },
                    {
                        id: 2,
                        title: "Tujuan Kami",
                        content: `
                            1. Rumah sakit umum dengan unggulan dalam pelayanan medis khususnya Bidang Bedah dan Anak.
                            2. Rumah sakit umum yang mengutamakan pelayanan prima (service excellence).
                        `
                    },
                    {
                        id: 3,
                        title: "Misi Kami",
                        content: `
                            1. Menyelenggarakan Pelayanan Medik, Keperawatan dengan Standar Profesional yang Setingkat Internasional.
                            2. Memberikan Pelayanan yang Bermutu, Nyaman, Aman, Ramah, Efektif dan Efisien.
                            3. Memfasilitasi Pelatihan Medis dan Keperawatan terutama Kasus Bedah dan Anak.
                        `
                    },
                    {
                        id: 3,
                        title: "Motto Kami",
                        content: `
                            MELAYANI SEPENUH HATI
                        `
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