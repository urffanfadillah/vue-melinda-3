<template>    
    <section class="container-fluid blue-theme p-5">
        <HeadingContent 
            white_title
            subTitle="RS Melinda 2"
            title="Hospital Plan"
        />
        <div class="cotainer mx-auto row">
            <div class="col-sm-4 border py-4 d-flex justify-content-center flex-column align-items-center">
                <span class="content-sub-title mb-1">Luas Tanah</span>
                <h1 class="heading fw-bold mb-4 text-white">3000<span class="fw-light">m2</span></h1>                
            </div>
            <div class="col-sm-4 border py-4">
                <span class="content-sub-title mb-1">Basement 2</span>
                <h1 class="heading fw-bold mb-4 text-white">B2</h1> 
                <p class="fw-light text-white">
                    Area Parkir, Ruang Jenazah
                </p>
            </div>
            <div class="col-sm-4 border py-4">
                <span class="content-sub-title mb-1">Basement 1</span>
                <h1 class="heading fw-bold mb-4 text-white">B1</h1> 
                <p class="fw-light text-white">
                    Area Parkir, Mushola, Minimart
                </p>
            </div>
            <div class="col-sm-4 border py-4">                
                <h1 class="heading fw-bold mb-4 text-white">L</h1> 
                <p class="fw-light text-white">
                    Public Area, Main Lobby, Farmasi/Apotek, Laboratorium, IGD, Information, Admission, Kasir, Playground, Klinik Orthopedi, Endoskopi, Radiologi, Rekam Medis, Cafetaria, Store, ATM, Bank Anda, Ruang Tunggu.
                </p>
            </div>
            <div class="col-sm-4 border py-4">                
                <h1 class="heading fw-bold mb-4 text-white">1</h1> 
                <p class="fw-light text-white">
                    Laboratorium, Klinik Anak, Klinik Obgyn, Klinik Mata, Klinik THT, Klinik Gigi, Klinik Gastroenterology, Klinik Bedah Digestif, Klinik Bedah Anak, Klinik Bedah Oncologi, Kamar Rawat Inap, Farmasi/Apotek,  Kasir, Store, Ruang Tunggu.
                </p>
            </div>
            <div class="col-sm-4 border py-4">                
                <h1 class="heading fw-bold mb-4 text-white">2</h1> 
                <p class="fw-light text-white">
                    Kamar Rawat Inap
                </p>
            </div>
            <div class="col-sm-4 border py-4">                
                <h1 class="heading fw-bold mb-4 text-white">3</h1> 
                <p class="fw-light text-white">
                    NICU, PICU, ICU, HCU, Nursery, ODS, Kamar Operasi, Kamar Rawat Inap, CSSD.
                </p>
            </div>
            <div class="col-sm-4 border py-4">                
                <h1 class="heading fw-bold mb-4 text-white">UB</h1> 
                <p class="fw-light text-white">
                    Rehabilitasi Medis, Gymnasium, HydroTherapy, Child Development Centre (CDC), Bandung Urologi Center, ESWL, Sistoskopi, Urodinamic, Hemodialisa, Cafetaria, Kantor Manajemen.
                </p>
            </div>
            <div class="col-sm-4 border py-4">                
                <h1 class="heading fw-bold mb-4 text-white">6</h1> 
                <p class="fw-light text-white">
                    Laboratorium IVF, Auditorium, Guest House, Mushola, Ruang Tunggu, Lounge.
                </p>
            </div>
        </div>
    </section>
</template>

<script>
    import HeadingContent from "@/components/utils/HeadingContent.vue"
    export default {    
        components: {
            HeadingContent
        }    
    }
</script>

<style scoped>
    .blue-theme {
        background: #1B4674;
    }
</style>