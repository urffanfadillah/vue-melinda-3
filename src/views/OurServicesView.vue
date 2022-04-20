<script>
    import FooterContent from "@/components/utils/FooterContent.vue"
    import ContentImages from "@/components/utils/ContentImages.vue"
    import HeroText from "@/components/utils/HeroText.vue"
    import HeadingContent from "@/components/utils/HeadingContent.vue"
    export default {
        components: {
            FooterContent, HeroText, ContentImages, HeadingContent
        }
    }
</script>

<template>
    <HeroText 
        subTitle="Our Great Services" 
        title="Our Services" 
        content="Various health facilities with state-of-the-art medical equipment and the latest. Making the quality of hospital services the best, safe, comfortable, friendly, effective, and efficient."
        blueTheme
    />
    <div class="container mx-auto py-4">
        <!-- input group -->
        <div class="input-group mb-3">
            <select class="form-select" aria-label="Default select example">
                <option value="Katerisasi Jantung" selected>Katerisasi Jantung</option>
                <option value="Two" selected>Two</option>
                <option value="Three" selected>Three</option>
            </select>
            <input v-model="search" type="text" class="form-control" id="basic-url" aria-describedby="basic-addon3" placeholder="Cari disini...">
            <button class="btn btn-outline-secondary py-3 btn-search" type="button" id="button-addon2">
                Search Services
            </button>
        </div>
    </div>
    <!-- Service -->
    <ContentImages noBackground
        subTitle="RS Melinda 2 Services"
        title="Disgestive Surgery"
        paragraph="Sed ut perspiciatis unde omnis iste natus error sit voluptatem 
        accusantium doloremque laudantium, totam rem aperiam, eaque  ipsa quae ab illo inventore veritatis et quasi architecto beatae vitae dicta sunt explicabo."
    >
        <img src="https://dummyimage.com/800x500/000/fff" alt="services" class="img-fluid" style="object-fit: cover;">    
    </ContentImages>
    <!-- Service -->
    <ContentImages noBackground
        isSwaped
        subTitle="RS Melinda 2 Services"
        title="Urogynecology"
        paragraph="Sed ut perspiciatis unde omnis iste natus error sit voluptatem 
        accusantium doloremque laudantium, totam rem aperiam, eaque  ipsa quae ab illo inventore veritatis et quasi architecto beatae vitae dicta sunt explicabo."
    >
        <img src="https://dummyimage.com/800x500/000/fff" alt="services" class="img-fluid" style="object-fit: cover;">    
    </ContentImages>
    <div class="container-fluid background-cream">
      <div class="container py-5 row mx-auto">
        <div class="col-sm-6">
          <HeadingContent
            blue_title
            text_dark
            subTitle="RS Melinda 2 Services" 
            title="Emergency Unit"
            paragraph="Sed ut perspiciatis unde omnis iste natus error sit voluptatem 
            accusantium doloremque laudantium, totam rem aperiam, eaque  ipsa quae ab illo inventore veritatis et quasi architecto beatae  vitae dicta sunt explicabo." />
        </div>
        <div class="col-sm-6">
          <HeadingContent
            blue_title
            text_dark
            subTitle="RS Melinda 2 Services" 
            title="Bedah Saraf"
            paragraph="Sed ut perspiciatis unde omnis iste natus error sit voluptatem 
            accusantium doloremque laudantium, totam rem aperiam, eaque  ipsa quae ab illo inventore veritatis et quasi architecto beatae  vitae dicta sunt explicabo." />
        </div>
      </div>
    </div>
    <!-- Service -->
    <ContentImages noBackground        
        subTitle="RS Melinda 2 Services"
        title="Bedah Plastik & Rekonstruksi Estetik"
        paragraph="Sed ut perspiciatis unde omnis iste natus error sit voluptatem 
        accusantium doloremque laudantium, totam rem aperiam, eaque  ipsa quae ab illo inventore veritatis et quasi architecto beatae vitae dicta sunt explicabo."
    >
        <img src="https://dummyimage.com/800x500/000/fff" alt="services" class="img-fluid" style="object-fit: cover;">    
    </ContentImages>
    <!-- Service -->
    <ContentImages noBackground
        isSwaped        
        subTitle="RS Melinda 2 Services"
        title="Pediatric Surgery"
        paragraph="Sed ut perspiciatis unde omnis iste natus error sit voluptatem 
        accusantium doloremque laudantium, totam rem aperiam, eaque  ipsa quae ab illo inventore veritatis et quasi architecto beatae vitae dicta sunt explicabo."
    >
        <img src="https://dummyimage.com/800x500/000/fff" alt="services" class="img-fluid" style="object-fit: cover;">    
    </ContentImages>
    <!-- Service -->
    <ContentImages noBackground        
        subTitle="RS Melinda 2 Services"
        title="Orthoepaedic & Traumatology Center"
        paragraph="Sed ut perspiciatis unde omnis iste natus error sit voluptatem 
        accusantium doloremque laudantium, totam rem aperiam, eaque  ipsa quae ab illo inventore veritatis et quasi architecto beatae vitae dicta sunt explicabo."
    >
        <img src="https://dummyimage.com/800x500/000/fff" alt="services" class="img-fluid" style="object-fit: cover;">    
    </ContentImages>
    <!-- Service -->
    <ContentImages noBackground
        isSwaped        
        subTitle="RS Melinda 2 Services"
        title="Bandung Urology Center"
        paragraph="Sed ut perspiciatis unde omnis iste natus error sit voluptatem 
        accusantium doloremque laudantium, totam rem aperiam, eaque  ipsa quae ab illo inventore veritatis et quasi architecto beatae vitae dicta sunt explicabo."
    >
        <img src="https://dummyimage.com/800x500/000/fff" alt="services" class="img-fluid" style="object-fit: cover;">    
    </ContentImages>
    <!-- Service -->
    <ContentImages noBackground                
        subTitle="RS Melinda 2 Services"
        title="Oncology Surgery"
        paragraph="Sed ut perspiciatis unde omnis iste natus error sit voluptatem 
        accusantium doloremque laudantium, totam rem aperiam, eaque  ipsa quae ab illo inventore veritatis et quasi architecto beatae vitae dicta sunt explicabo."
    >
        <img src="https://dummyimage.com/800x500/000/fff" alt="services" class="img-fluid" style="object-fit: cover;">    
    </ContentImages>
    <FooterContent/>    
</template>

<style scoped>
    .btn-search {
        background: #75C6EF;
        border: transparent;
        color: #ffffff;
    }
    .btn-search:hover {
        opacity: 0.5;
        background: #75C6EF;
        border: transparent;
        color: #ffffff;
    }
    .konten {
        padding: 48px 10% 48px 10%;     
    }

    .no-background {
        background-color: #ffffff00;
    }
    .background-blue {
        background-color: #1B4674;
    }

    .background-cream {
        background-color: #FDF4E9;
    }
    p.fw-light {
        line-height: 150%;
        color: #575757;
    }
    #hero-images-homepage {
        width: 50%;    
        display: block;    
    }

    .wrapper-hero-img {
        margin-top: -30%;
        z-index: 998;
        display: flex;
        justify-content: end;    
    }

    .mouse {
        width: 34px;
    }

    .bg-img-1 {
        height: 460px;
        background-image: url("@/assets/images/services-img-3.png");
        background-size: cover;
        object-fit: cover;    
    }

    .bg-img-2 {
        height: 460px;
        background-image: url("@/assets/images/services-img-4.png");
        background-size: cover;
        object-fit: cover;    
    }

    .bg-img-1 p, .bg-img-2 p {
        color: white !important;
        z-index: 1000;
        filter: brightness(100%) !important;
    }

    @media (max-width: 575px) {
        .wrapper-hero-img {
            margin-top: 0;
            z-index: 0;
            display: none;
            justify-content: end;    
        }
    }

    @media (max-width: 1199.98px) {
        .wrapper-hero-img {
            margin-top: 0;
            z-index: 0;
            display: flex;
            justify-content: end;    
        }
    }
</style>