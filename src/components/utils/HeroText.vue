<template>    
  <section class="d-block" :class="{'blue-theme':blueTheme}">
      <div class="container d-flex justify-content-start flex-column links-hero gap-2 py-5">
        <span class="content-sub-title text-start">{{subTitle}}</span>
        <h1 class="content-title text-start" :class="{'text-white':blueTheme}" >
            {{title}}
        </h1>
        <p class="text-start links-desc" :class="{'text-white':blueTheme}">
            {{content}}
        </p>
      </div>
  </section>
</template>

<script>
    export default {
        props: {
            title: String,
            subTitle: String,
            content: String,
            blueTheme: Boolean
        }
    }
</script>

<style scoped>
    .blue-theme {
        background-color: #1B4674;
    }
</style>