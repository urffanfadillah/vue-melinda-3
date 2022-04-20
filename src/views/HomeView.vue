<script>
  import JumbotronComps from "@/components/home/JumbotronComps.vue"
  import HeadingContent from "@/components/utils/HeadingContent.vue"
  import ContentImages from "@/components/utils/ContentImages.vue"
  import CarouselComps from "@/components/home/CarouselComps.vue"
  import ArticlesComps from "@/components/home/ArticlesComps.vue"
  import FooterContent from "@/components/utils/FooterContent.vue"
  export default {
    name: 'HomeView',
    components: { JumbotronComps, HeadingContent, ContentImages, CarouselComps, ArticlesComps, FooterContent },
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
    <!-- List Services -->
    <div class="container-fluid background-cream">
      <div class="container py-5 row mx-auto">
        <div class="col-sm-6">
          <HeadingContent 
            subTitle="Stay strong and lets beat Cervical Cancer!" 
            title="Our Great Services for Your Family Care" 
          >
            <a href="#" data-bs-toggle="modal" data-bs-target="#auth" class="btn-pendaftaran btn btn-primary rounded-pill">
                View All Services <i class="bi bi-arrow-right"></i>
            </a>
          </HeadingContent>
        </div>
        <div class="col-sm-6 row">
          <div class="col-sm-6" v-for="listService in listServices" :key="listService">
            <p class="text-services fw-bold">
              {{listService}}
            </p>
          </div>
        </div>
      </div>
    </div>
    <!-- /List Services -->
    <ContentImages 
      title="Our First Facility Surgery & Kids Center" 
      paragraph="Dilengkapi dengan berbagai fasilitas kesehatan, di antaranya : Orthopaedics & Traumatologi Center, Bandung Urologi Center"
    >
      <img src="https://dummyimage.com/600x400/000/fff" class="d-block mx-auto img-fluid" alt="Bootstrap Themes" style="width: 100%;" height="500" loading="lazy">
        <template v-slot:extra>
          <a href="#" class="btn-pendaftaran btn btn-primary rounded-pill">
              View All Services <i class="bi bi-arrow-right"></i>
          </a>
      </template>
    </ContentImages>
    <!-- carousel -->
    <CarouselComps />
    <!-- /carousel -->
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