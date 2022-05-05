<script>
    import HeadingContent from "@/components/utils/HeadingContent.vue"
    export default {
        components: {
            HeadingContent
        },
        data() {
            return {
                filterSpecialist: 'Semua',
                search: '',          
                doctors: [                                        
                    {
                        specialist: "Dokter Spesialis Kandungan",
                        dataDoctor: [
                            { id: 1, name:"dr. Susan Melinda, Sp. OG", imgUrl: "https://dummyimage.com/600x400/000/fff" },
                            { id: 2, name:"Dr. dr. H. Rono.S.H, Sp.OG(K), MM", imgUrl: "https://dummyimage.com/600x400/000/fff" },
                            { id: 3, name:"dr. Julius T. Pangayoman, Sp.OG", imgUrl: "https://dummyimage.com/600x400/000/fff" },
                            { id: 4, name:"Prof. Dr. dr. Vita M T, Sp.OG, SH, M.Kes, AIFO", imgUrl: "https://dummyimage.com/600x400/000/fff" },
                            { id: 5, name:"John Doe", imgUrl: "https://dummyimage.com/600x400/000/fff" }
                        ]
                    },
                    {
                        specialist: "Dokter Spesialis Bedah",
                        dataDoctor: [
                            { id: 6, name:"dr. Dradjat R. Suardi, SpB(K)-Onk, FICS", imgUrl: "https://dummyimage.com/600x400/000/fff" },
                            { id: 7, name:"dr. Concepcion Garcia, Sp.B", imgUrl: "https://dummyimage.com/600x400/000/fff" },
                            { id: 8, name:"dr. Johanes Casay Chandrawinata, MND, SpGK", imgUrl: "https://dummyimage.com/600x400/000/fff" },
                            { id: 9, name:"John Doe", imgUrl: "https://dummyimage.com/600x400/000/fff" }
                        ]
                    },
                    {
                        specialist: "Dokter Spesialis Anak",
                        dataDoctor: [
                            { id: 10, name:"dr. Tetty Yuniati, Sp.A(K), M.Kes", imgUrl: "https://dummyimage.com/600x400/000/fff" },
                            { id: 11, name:"dr. Yulia Suryakusuma, Sp.A, M.Kes", imgUrl: "https://dummyimage.com/600x400/000/fff" }
                        ]
                    },
                ],             
            }
        },
    }
</script>

<template>
    <div class="container-fluid header bg-red row mx-0 px-0">
        <div class="col-sm-6 mt-5 px-5">
            <HeadingContent 
                white_title
                subTitle="RS Melinda Heart Center" 
                title="Protect The Beating of Every Heart" 
                paragraph="Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.">
                <a href="#" class="btn-readmore btn btn-primary rounded-pill">
                    Read More
                </a>
            </HeadingContent>
        </div>
        <div class="col-sm-6 bg-image d-none d-md-block">
            <p class="visually-hidden">p</p>
        </div>
    </div>
    <!-- input group desktop -->
    <div class="px-5 d-flex flex-column input-contact d-none d-md-block">
        <div class="input-group mb-3">
            <select class="form-select" aria-label="Default select example" name="filterSpecialist" v-model="filterSpecialist">
                <option value="Semua" selected>Semua</option>
                <option v-for="doctor in doctors" :key="doctor.specialist" v-bind:value="doctor.specialist">
                    {{doctor.specialist}}
                </option>                
            </select>
            <input v-model="search" type="text" class="form-control" id="basic-url" aria-describedby="basic-addon3" placeholder="Cari disini...">
            <button class="btn btn-outline-secondary py-3 btn-search-doctor" type="button" id="button-addon2">
                Search Doctor dan Schedule
            </button>        
        </div>
        <div class="gap-4 col-sm-12 py-4 d-flex flex-column flex-md-row">
            <div class="align-self-center d-flex align-items-center gap-4">
                <i class="bi bi-telephone fs-3 text-white"></i>
                <div class="d-flex flex-column">
                    <p class="fw-bold m-0 text-white">Hotline & Emergency Case</p>
                    <p class="fw-light m-0 text-white">08157100888</p>
                </div>
            </div>
            <div class="align-self-center d-flex align-items-center gap-4">
                <i class="bi bi-clock fs-3 text-white"></i>
                <div class="d-flex flex-column">
                    <p class="fw-bold m-0 text-white">Opening Hours</p>
                    <p class="fw-light m-0 text-white">24 Hours</p>
                </div>
            </div>                  
        </div> 
    </div>   
</template>

<style scoped>
    .input-contact {
        margin-top: -160px;
    }
    .btn-search-doctor {
        background: #1B4674;
        border: transparent;
        color: #ffffff;
    }
    .btn-search-doctor:hover {
        opacity: 0.5;
        background: #1B4674;
        border: transparent;
        color: #ffffff;
    }
    .btn-readmore {
        background: #FCE8CE;
        color: #474747;
        border: transparent;
    }
    .btn-readmore:hover {
        background: #FCE8CE;
        color: #474747;
        opacity: 0.5;
    }
    .header {
        height: 80vh;
    }
    .bg-image {
        background-image: url('@/assets/images/hero-melinda-3.png') !important;
        background-size: cover;
        object-fit: cover;
    }
    .bg-red {
        background: #CD4051;
    }
    @media (max-width: 575px) {
    .header {
        height: 40vh;
    }
    }   
</style>