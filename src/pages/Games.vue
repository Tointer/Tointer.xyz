<template>
  <Layout>
    <div>
      <h1 class="display-2 serif-font-face">Games We Created</h1>
        <div>
            <section class="card-columns">
                <Card  v-for="edge in games" :key="edge.id" :card="edge.game"/>
            </section>
        </div>
    </div>
  </Layout>
</template>

<page-query>
    query {
        allInstagramPhoto {
            edges {
                node {
                    display_url
                    edge_media_to_caption {
                        edges {
                            node {
                                text
                            }
                        }
                    }
                }
            }
        }
    }
</page-query>
<script>
    import Card from "../components/portfolio/Card";
    export default {
        components: {Card},
        metaInfo: {
            title: 'Games'
        },
        data() {
            return {
                games: [
                    {
                        id: 'puck',
                        game: {
                            to: 'sling-pucky',
                            img: '/Logo1024x1024.png',
                            text: 'Our new game Puck Sling!'
                        }
                    }
                ]
            }
        },
    }
</script>
