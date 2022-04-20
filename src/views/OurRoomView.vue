<script>
    import FooterContent from "@/components/utils/FooterContent.vue"    
    import CardRooms from "@/components/our-room/CardRooms.vue"
    import ExperienceRoom from "@/components/our-room/ExperienceRoom.vue"
    import HeroText from "@/components/utils/HeroText.vue"
    export default {
        components: {
            FooterContent, CardRooms, ExperienceRoom, HeroText
        }
    }
</script>

<template>
    <HeroText
      blueTheme
      subTitle="Best Room & Comfort"
      title="Our Room"
      content="Various health facilities with state-of-the-art medical equipment and the latest. Making the quality of hospital services the best, safe, comfortable, friendly, effective, and efficient."
    />
    <CardRooms />
    <ExperienceRoom />
    <FooterContent />
</template>