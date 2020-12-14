<template>
  <Layout>

    <div class="row">
      <div class="col-md-4">
        <h1 class="display-4 serif-font-face">Super Duper Creative Game Studio</h1>
        <p class="font-big-1">We believe that our games give so much pleasure to play.</p>
        <p class="font-big-1"><a href="#" class="text-dark font-weight-bold"><u>inboxforcom@gmail.com</u></a></p>
      </div>
      <div class="col-md-8">
        <Carousel :slides="slides" />
      </div>
    </div>
    <div class="p-5 bg-light my-3">
      <h1 class="serif-font-face">"Sling Pucky is inspired by board game "Sling Puck", where you should use sling rope to slam all pucks to the opponent side.</h1>
    </div>

  </Layout>
</template>

<script>
    import Carousel from "../components/home/Carousel";
    export default {
        components: {Carousel},
        metaInfo: {
            title: 'Home'
        },
        data() {
            return {
                slides: [
                    {
                        type: 'Production',
                        title: 'Game Release',
                        src: '/Logo1024x1024.png',
                        description: 'So here we introduce our Sling Pucky game!'
                    },
                    {
                      type: 'Development',
                      title: 'Game Dev',
                      src: '/GameTitle.png',
                      description: 'Game dev'
                    }
                ]
            }
        }
    }
</script>

<style>
  .home-links a {
    margin-right: 1rem;
  }
</style>