<script>
  import JumbotronComps from "@/components/home/JumbotronComps.vue"
  import ArticlesComps from "@/components/home/ArticlesComps.vue"
  import FooterContent from "@/components/utils/FooterContent.vue"
  export default {
    name: 'HomeView',
    components: { JumbotronComps, ArticlesComps, FooterContent },
    data() {
      return {
        listServices: [
          'UGD (Unit Gawat Darurat)',
          'Pediatric Surgery',
          'Bedah Saraf',
          'Urologi Pediatric',
          'Bedah Plastic dan Rekonstruksi Estetik',
          'Urologi Perempuan',
          'Pediatric Neonatology',
          'Pediatric Neonatology',
          'Urogynecology',
          'Urogynecology'
        ]
      }
    }
  }
</script>

<template>
    <JumbotronComps />
    <!-- articles -->
    <ArticlesComps />
    <!-- footer -->
    <FooterContent />
</template>

<style scoped>  
  .btn-pendaftaran, .link-to-readmore {
      background: #75C6EF;
      border: transparent;       
  }
  .btn-pendaftaran:hover {
      background: #75C6EF;
      border: transparent;
      opacity: 0.5;       
  }
  .text-services {
    color: #1B4674;
  }
</style>