<template>    
    <ContentImages
        noBackground                
        subTitle="Melinda Hospital"
        title="History of RS Melinda 2"
        paragraph="Rumah Sakit Melinda 2 terletak di pusat kota Bandung yang strategis, yaitu di Jl. Dr Cipto No.1 Bandung. Rumah Sakit Melinda 2 merupakan rumah sakit umum yang memiliki pelayanan yang unggul, baik di  dalam bidang medis maupun non-medis.

        Profesionalisme yang tinggi, kerja keras, kedisiplinan, serta kerja sama tim yang baik mampu menghasilkan kesuksesan untuk Rumah Sakit Melinda 2 dalam memenuhi standar Internasional, baik dalam kesehatan maupun keselamatan pasien.

        Rumah Sakit Melinda 2, hadir sejak Juni 2014. Rumah Sakit Melinda 2 memiliki bangunan lima lantai dan dua basement yang luas totalnya mencapai 3000 meter persegi.

        Rumah Sakit Melinda 2 menyediakan berbagai fasilitas kesehatan dengan peralatan medis yang canggih dan terbaru, serta didukung oleh staf medis yang profesional untuk mengoperasikan peralatan tersebut. Selain itu, Rumah Sakit Melinda 2 memiliki lebih dari  90 dokter dan staff ahli serta 140 perawat yang selalu siaga untuk membantu pasien.

        Sebagai rumah sakit yang menyediakan pelayanan yang profesional, Rumah Sakit Melinda 2 menganggap sumber daya manusia sebagai sumber daya yang utama dalam pelayanan. Oleh karena itu, Rumah Sakit Melinda 2 memiliki komitmen yang kuat untuk meningkatkan kemampuan dan profesionalisme sumber daya manusianya melalui pendidikan dan pelatihan rutin yang dilakukan secara terus menerus, baik di dalam maupun di luar negeri.

"        
    >
        <img src="@/assets/images/group-about.png" alt="services" class="img-fluid" style="object-fit: cover;">
    </ContentImages>
    <VisiMisi />   
    <ContentImages
        noBackground
        isSwaped
        subTitle="RS Melinda 2 Services"
        title="Kebijakan Mutu"
        paragraph="Rumah Sakit Melinda 2 berkomitmen memberikan pelayanan sesuai standar mutu
        serta sistem keselamatan pasien dan manajemen risiko
        sehingga memberikan rasa aman dan nyaman
        sesuai harapan pengguna jasa maupun pekerja di lingkungan rumah sakit"        
    >
        <img src="https://dummyimage.com/800x400/000/fff" alt="services" class="img-fluid" style="object-fit: cover;">
    </ContentImages>
    <div class="container mx-auto py-5">
        <HeadingContent 
            subTitle="Melinda Hospital"
            title="Our Filosofy"
        />        
        <div class="row">
            <div class="col-sm-12">
                <p>
                    Melinda Hospital was established on July 23, 2004, and during that time the concept and pattern of serving wholeheartedly was sown, implanted, nurtured, nurtured and fought for until now.

                    Serving must be wholehearted and accompanied by sincere thoughts, feelings and wills. The personality of an employee in serving patients totally or wholeheartedly is believed to have a positive impact on the patient's healing, body and soul, as well as the spirit of life, attitudes, and behavior of the patient.

                    This heart-based service process is also related to the formation of employee character. By serving wholeheartedly directly and concretely to patients, there is a change in employees, strengthening their mindset, attitude patterns, and positive behavior patterns. One example is that employees become more optimistic at work, broad-minded, more patient and able to control emotions, and are more positive-minded.

                    This heart-based service is also believed to have a positive impact on the image of the institution, in this case Melinda Hospital, contributing to improving the image of the world of Indonesian hospitals in the international arena.
                </p>
                <p>
                    Serving wholeheartedly can fail if employees and doctors are not sensitive to patient needs, are not friendly to patients, and do not apologize for disappointing patients. The most fatal attitude from patients is when doctors and employees are considered the cause of discomfort or disappointment. This will spread to the image of the institution that was originally glorified and could turn 180 degrees into scorn, abandonment and even alienation, not wanting to hear anymore.

                    Getting into the habit of serving wholeheartedly requires willingness, and serious effort and serious commitment, taking into account real practices, including the following:

                    Be willing to listen with empathy.
                    Willing to take the time to answer and discuss using various media, including cyberspace.
                    Maintain a communication relationship with the spirit of openness, warmth, and ethics.
                    Counseling, motivation, and enthusiasm for life.
                    Tenderness and do a touch of love to the patient.
                    In summary, serve wholeheartedly, the first is always grateful, the second does not forget to always be grateful for the trust of our customers, the third is to apologize for our shortcomings and mistakes as imperfect humans.
                </p>
            </div>
        </div>
    </div>
    <HospitalPlan />
    <FooterContent />
</template>

<script>
    import VisiMisi from "@/components/about/VisiMisi.vue"
    import ContentImages from "@/components/utils/ContentImages.vue"
    import HeadingContent from "@/components/utils/HeadingContent.vue"
    import FooterContent from "@/components/utils/FooterContent.vue"
    import HospitalPlan from "@/components/about/HospitalPlan.vue"
    export default {
        components: {
            ContentImages, HeadingContent, FooterContent, VisiMisi, HospitalPlan
        }
    }   
</script>

<style>

</style>