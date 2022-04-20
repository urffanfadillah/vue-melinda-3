<script>
    import FooterContent from "@/components/utils/FooterContent.vue"        
    import HeadingContent from "@/components/utils/HeadingContent.vue"
    export default {
        components: {
            FooterContent,                        
            HeadingContent
        }
    }
</script>

<template>
   <section class="mx-0 px-0 container-fluid row">
        <div class="col-sm-12 row mx-0 px-0">
            <div class="col-sm-7 bg-link-img-3"></div>
            <div class="col-sm-5 content-melinda-3">
                <HeadingContent 
                    text_dark
                    title="Story in Every Place"
                    subTitle="Melinda Hospital Gallery"
                    paragraph="Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi architecto beatae vitae dicta sunt explicabo. "
                    blue_title
                >
                    <a href="/gallery-detail" class="link-to-website btn btn-light text-white">
                       View Gallery <i class="bi bi-arrow-right"></i>
                    </a>
                </HeadingContent>
            </div>
        </div>
        <div class="col-sm-12 row mx-0 px-0">
            <div class="col-sm-5 content-melinda-3">
                <HeadingContent 
                    text_dark
                    title="Story in Every Place"
                    subTitle="Melinda Hospital Gallery"
                    paragraph="Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi architecto beatae vitae dicta sunt explicabo. "
                    blue_title
                >
                    <a href="/gallery-detail" class="link-to-website btn btn-light text-white">
                       View Gallery <i class="bi bi-arrow-right"></i>
                    </a>
                </HeadingContent>
            </div>
            <div class="col-sm-7 bg-link-img-2"></div>
        </div>
        <div class="col-sm-12 row mx-0 px-0">
            <div class="col-sm-7 bg-link-img-3"></div>
            <div class="col-sm-5 content-melinda-3">
                <HeadingContent 
                    text_dark
                    title="Story in Every Place"
                    subTitle="Melinda Hospital Gallery"
                    paragraph="Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi architecto beatae vitae dicta sunt explicabo. "
                    blue_title
                >
                    <a href="/gallery-detail" class="link-to-website btn btn-light text-white">
                       View Gallery <i class="bi bi-arrow-right"></i>
                    </a>
                </HeadingContent>
            </div>
        </div>
    </section>
    <FooterContent />
</template>

<style scoped>
    #link-other {
        padding: 160px 80px;
    }

    .link-to-website {
        border-radius: 40px;
        background-color: #75C6EF;
        padding: 8 16px 8 16px;
        font-size: 14px;
        border: none;
    }
    
    .link-to-website:hover {
        border-radius: 40px;
        background-color: #57add8;
        padding: 8 16px 8 16px;
        font-size: 14px;
        border: none;
    }

    .konten {
        padding: 48px 10% 48px 10%;     
    }

    .background-cream {
        background-color: #FDF4E9;
    }
    p.fw-light {
        line-height: 150%;
        color: #575757 !important;
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

    .bg-link-img-2 {        
        background-image: url("@/assets/images/melinda-1.png");
        background-size: cover;
        object-fit: cover;    
        padding: 120px 0 120px 60px;
    }
    
    .bg-link-img-3 {        
        background-image: url("@/assets/images/melinda-2.png");
        background-size: cover;
        object-fit: cover;            
    }

    .content-melinda-3 {
        padding: 120px 60px 120px 60px;
        background-color: #ffffff;        
    }

    .links-desc {
        width: 60%;
        margin: 0 auto;
    }

    .card-link {
        position: relative;
    }

    .card-link-body {
        position: absolute;
        bottom: 8px;
        left: 16px;
    }

    .card-link-body p {
        color: #575757;
        width: 100% !important;
        font-size: 20px;
        font-weight: bold !important;    
    }

    .links-hero { padding: 80px 0 80px 0; }

    @media (max-width: 575px) {
        .wrapper-hero-img {
            margin-top: 0;
            z-index: 0;
            display: none;
            justify-content: end;    
        }
        .links-desc {
            width: 90%;
            margin: 0 auto;
        }
        .bg-link-img-2 {        
            background-image: url("@/assets/images/bg-link-1.png");
            background-size: cover;
            object-fit: cover;    
            padding: 120px 0 120px 0px;
        }
        #link-other {
            padding: 80px 20px;
        }
    }

    @media (max-width: 1199.98px) {
        #link-other {
            padding: 80px 40px;
        }
        .wrapper-hero-img {
            margin-top: 0;
            z-index: 0;
            display: flex;
            justify-content: end;    
        }
        .links-desc {
            width: 80%;
            margin: 0 auto;
        }
        .bg-link-img-2 {        
            background-image: url("@/assets/images/bg-link-1.png");
            background-size: cover;
            object-fit: cover;    
            padding: 120px 0 120px 0px;
        }
    }
</style>