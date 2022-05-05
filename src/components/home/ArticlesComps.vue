<template>
    <div class="container hospital-nearby my-4">
        <div class="text-center mb-5">
            <h2>News & Articles</h2>
            <p>
                Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
            </p>
            <div class="border-red mx-auto"></div>
        </div>
        <div class="row">
            <div class="col-sm-6">
                <div class="col-sm-12" v-for="article in articles.slice(0,2)" v-bind:key="article.id">
                    <div class="card mb-3" style="max-width: 540px;">
                        <div class="row g-0">
                            <div class="col-md-4">
                                <img v-bind:src="article.imgSrc" class="img-fluid rounded-start" alt="articles">
                            </div>
                            <div class="col-md-8">
                                <div class="card-body">
                                    <span class="badge bg-primary">{{article.tags}}</span>
                                    <h5 class="card-title">
                                        <!-- <a href="article-detail/">{{article.title}}</a> -->
                                        <router-link :to="{ name: 'artikel', params: { id: article.id } }" >{{article.title}}</router-link>
                                    </h5>
                                    <span class="text-light">{{article.date}}</span>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
            <div class="col-sm-6 align-self-stretch">
                <div class="col-sm-12" v-for="article in articles.slice(2)" v-bind:key="article.id">
                    <div class="card bg-dark text-white">
                        <img v-bind:src="article.imgSrc" class="card-img" alt="article">
                        <div class="card-img-overlay">
                            <span class="badge bg-primary">{{article.tags}}</span>
                            <h5 class="card-title">
                                <!-- <a href="article-detail/">{{article.title}}</a> -->
                                <router-link :to="{ name: 'artikel', params: { id: article.id } }" >{{article.title}}</router-link>
                            </h5>
                            <span class="text-light">{{article.date}}</span>
                        </div>
                    </div>
                </div>
            </div>
        </div>  
    </div>
</template>

<script>
    export default {
        data() {
            return {
                articles: [
                    { 
                        id: 1,
                        tags:"Tips & Healthy", 
                        title:"Tips Mengurangi Resiko Gejala Covid-19", 
                        date:"12 Januari 2021", 
                        imgSrc:"https://dummyimage.com/600x700/000/fff",
                        url:"https://google.com",
                        content: `In 2004 ago, dr. Susan Melinda, SpOG., a specialist in obstetrics and gynecology, established a hospital with the concept of a 5-star hotel and an art gallery that offers health facilities for women, especially mothers and children.

                        under the name Melinda Hospital. With an international standard, the hospital, which was established on July 23, 2004, is equipped with professional medical personnel. "Health is the main key to a woman's beauty and happiness. We are sincerely committed to realizing every woman's dream to look beautiful, healthy and happy." said dr. Susan Melinda about her concern for women's needs.

                        As a hospital devoted to women, Melinda Hospital was built so that all women can express their noble side, whether they are in a position as a woman or as a mother to their children. With a unique hospital concept, it will make patients and visitors feel comfortable. Melinda Hospital consists of five floors with a capacity of 33 beds, modern, energy efficient, minimalist architecture, spacious rooms and corridors. The Art & Craft Gallery which is installed along the corridor will also make the atmosphere warmer to welcome anyone who comes to Melinda Hospital.`                         
                    },
                    {
                        id: 2,
                        tags:"Corporate", 
                        title:"Fasilitas Terbaru di Melinda", 
                        date:"12 Januari 2021", 
                        imgSrc:"https://dummyimage.com/600x700/000/fff", 
                        url:"https://google.com",
                        content: `In 2004 ago, dr. Susan Melinda, SpOG., a specialist in obstetrics and gynecology, established a hospital with the concept of a 5-star hotel and an art gallery that offers health facilities for women, especially mothers and children.

                        under the name Melinda Hospital. With an international standard, the hospital, which was established on July 23, 2004, is equipped with professional medical personnel. "Health is the main key to a woman's beauty and happiness. We are sincerely committed to realizing every woman's dream to look beautiful, healthy and happy." said dr. Susan Melinda about her concern for women's needs.

                        As a hospital devoted to women, Melinda Hospital was built so that all women can express their noble side, whether they are in a position as a woman or as a mother to their children. With a unique hospital concept, it will make patients and visitors feel comfortable. Melinda Hospital consists of five floors with a capacity of 33 beds, modern, energy efficient, minimalist architecture, spacious rooms and corridors. The Art & Craft Gallery which is installed along the corridor will also make the atmosphere warmer to welcome anyone who comes to Melinda Hospital.`
                    },
                    {
                        id: 3,
                        tags:"Medical Care", 
                        title:"Teknologi Canggih Melinda Hospital", 
                        date:"12 Januari 2021", 
                        imgSrc:"https://dummyimage.com/600x700/000/fff",
                        url:"https://google.com",
                        content: `In 2004 ago, dr. Susan Melinda, SpOG., a specialist in obstetrics and gynecology, established a hospital with the concept of a 5-star hotel and an art gallery that offers health facilities for women, especially mothers and children.

                        under the name Melinda Hospital. With an international standard, the hospital, which was established on July 23, 2004, is equipped with professional medical personnel. "Health is the main key to a woman's beauty and happiness. We are sincerely committed to realizing every woman's dream to look beautiful, healthy and happy." said dr. Susan Melinda about her concern for women's needs.

                        As a hospital devoted to women, Melinda Hospital was built so that all women can express their noble side, whether they are in a position as a woman or as a mother to their children. With a unique hospital concept, it will make patients and visitors feel comfortable. Melinda Hospital consists of five floors with a capacity of 33 beds, modern, energy efficient, minimalist architecture, spacious rooms and corridors. The Art & Craft Gallery which is installed along the corridor will also make the atmosphere warmer to welcome anyone who comes to Melinda Hospital.` 
                    }
                ]
            }
        }
    }
</script>

<style>
    .border-red {
        border-bottom: 4px solid #CD4051;
        width: 60px;        
    }
    .card-article {
        position: relative;
    }

    .card-article-body {
        position: absolute;
        bottom: 8px;
        left: 16px;
    }

    .card-article-body h5 a {
        color: white;
        width: 100% !important;
        font-size: 20px;
        font-weight: bold !important;
        text-decoration: none;    
    }
    .card-article-body h5 a:hover {
        color: white;
        width: 100% !important;
        font-size: 20px;
        font-weight: bold !important;
        text-decoration: none;
        opacity: 0.5;    
    }
    @media (max-width: 1199.98px) {
        footer #contact {        
            padding: 48px 8% 48px 8%;
            justify-content: space-between;
            background-color: #FEF8F0;        
        }
        footer hr { width: 84%; }
    }
</style>