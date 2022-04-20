<template>
    <HeroText 
        blueTheme
        subTitle="Our Great Serivces"
        title="Disgestive Surgery"
        content="Various health facilities with state-of-the-art medical equipment and the latest. Making the quality of hospital services the best, safe, comfortable, friendly, effective, and efficient."
    />
    <ContentImages
        noBackground                
        paragraph="Depertemen Digestive Surgery (Bedah Digestif) melakukan prosedur bedah yang semuanya diakui secara internasional (baik laparoskopi dan klasik) dalam pengobatan penyakit jinak maupun ganas, kerongkongan, lambung dan usus besar, usus kecil dan usus besar, hati, dan kantong empedu, billiard tracks, pankreas, limpa, anal, dan perianal wilayah, hernia di dinding perut dan selangkangan."        
    >
        <img src="https://dummyimage.com/800x400/000/fff" alt="services" class="img-fluid" style="object-fit: cover;">
    </ContentImages>
    <FooterContent/>
</template>

<script>
    import FooterContent from "@/components/utils/FooterContent.vue"
    import HeroText from "@/components/utils/HeroText.vue"
    import ContentImages from "@/components/utils/ContentImages.vue"
    export default {
        components: {
            FooterContent, HeroText, ContentImages
        }
    }
</script>

<style>

</style>