<template>
  <Layout>
    <div class="container">
      <div class="hero">
        <h1 class="hero-title">{{general.title}}</h1>
        <h2 class="hero-subtitle">
          {{general.subtitle}}
        </h2>
      </div>
      <div data-v-50cbff3e="" class="projects">
         <div data-v-50cbff3e="" class="project" v-for="edge in $page.posts.edges" :key="edge.node.id">
          <a
            data-v-50cbff3e=""
            href="/"
            class="project-link"
            ><img
              data-v-50cbff3e=""
              :alt="`${edge.node.title}`"
              :src="`${GRIDSOME_API_URL}${edge.node.big_picture.url}`"
              width="2560"
              :data-src="`${GRIDSOME_API_URL}${edge.node.big_picture.url}`"
              data-sizes="(max-width: 2560px) 100vw, 2560px"
              class="thumbnail g-image g-image--lazy g-image--loaded"
              sizes="(max-width: 2560px) 100vw, 2560px"
            /><noscript data-v-50cbff3e=""
              ><img
                :src="`${GRIDSOME_API_URL}${edge.node.big_picture.url}`"
                class="thumbnail g-image g-image--loaded"
                width="2560"
                :alt="`${edge.node.title}`"
            /></noscript>
            <h3 data-v-50cbff3e="" class="project-title">{{edge.node.title}}</h3>
            <div data-v-50cbff3e="" class="categories">
              <span data-v-50cbff3e="" class="category">photography</span
              ><span data-v-50cbff3e="" class="category">{{edge.node.color}}</span>
            </div></a
          >
        </div>
        <!-- <div data-v-50cbff3e="" class="project">
          <a
            data-v-50cbff3e=""
            href="/projects/chelsea-landmark/"
            class="project-link"
            ><img
              data-v-50cbff3e=""
              alt="Banana"
              src="https://gridsome-forestry.netlify.app/assets/static/mike-dorner-173502-unsplash.c0dad42.16e7958f24c375d7bd7b08073b4ce000.jpg"
              width="2560"
              data-src="https://gridsome-forestry.netlify.app/assets/static/mike-dorner-173502-unsplash.c0dad42.16e7958f24c375d7bd7b08073b4ce000.jpg"
              data-srcset="https://gridsome-forestry.netlify.app/assets/static/mike-dorner-173502-unsplash.b6e36c6.16e7958f24c375d7bd7b08073b4ce000.jpg 480w, /assets/static/mike-dorner-173502-unsplash.1c9e94c.16e7958f24c375d7bd7b08073b4ce000.jpg 1024w, /assets/static/mike-dorner-173502-unsplash.f11e5e1.16e7958f24c375d7bd7b08073b4ce000.jpg 1920w, /assets/static/mike-dorner-173502-unsplash.c0dad42.16e7958f24c375d7bd7b08073b4ce000.jpg 2560w"
              data-sizes="(max-width: 2560px) 100vw, 2560px"
              class="thumbnail g-image g-image--lazy g-image--loaded"
              srcset="
                https://gridsome-forestry.netlify.app/assets/static/mike-dorner-173502-unsplash.b6e36c6.16e7958f24c375d7bd7b08073b4ce000.jpg  480w,
                https://gridsome-forestry.netlify.app/assets/static/mike-dorner-173502-unsplash.1c9e94c.16e7958f24c375d7bd7b08073b4ce000.jpg 1024w,
                https://gridsome-forestry.netlify.app/assets/static/mike-dorner-173502-unsplash.f11e5e1.16e7958f24c375d7bd7b08073b4ce000.jpg 1920w,
                https://gridsome-forestry.netlify.app/assets/static/mike-dorner-173502-unsplash.c0dad42.16e7958f24c375d7bd7b08073b4ce000.jpg 2560w
              "
              sizes="(max-width: 2560px) 100vw, 2560px"
            /><noscript data-v-50cbff3e=""
              ><img
                src="https://gridsome-forestry.netlify.app/assets/static/mike-dorner-173502-unsplash.c0dad42.16e7958f24c375d7bd7b08073b4ce000.jpg"
                class="thumbnail g-image g-image--loaded"
                width="2560"
                alt="Banana"
            /></noscript>
            <h3 data-v-50cbff3e="" class="project-title">Banana</h3>
            <div data-v-50cbff3e="" class="categories">
              <span data-v-50cbff3e="" class="category">photography</span
              ><span data-v-50cbff3e="" class="category">pink</span>
            </div></a
          >
        </div>
        <div data-v-50cbff3e="" class="project">
          <a data-v-50cbff3e="" href="/projects/sunk/" class="project-link"
            ><img
              data-v-50cbff3e=""
              alt="Pineapple"
              src="https://gridsome-forestry.netlify.app/assets/static/cody-davis-253925-unsplash.c0dad42.ce547449449f5efa1a8b8f02c7abb04d.jpg"
              width="2560"
              data-src="https://gridsome-forestry.netlify.app/assets/static/cody-davis-253925-unsplash.c0dad42.ce547449449f5efa1a8b8f02c7abb04d.jpg"
              data-srcset="https://gridsome-forestry.netlify.app/assets/static/cody-davis-253925-unsplash.b6e36c6.ce547449449f5efa1a8b8f02c7abb04d.jpg 480w, /assets/static/cody-davis-253925-unsplash.1c9e94c.ce547449449f5efa1a8b8f02c7abb04d.jpg 1024w, /assets/static/cody-davis-253925-unsplash.f11e5e1.ce547449449f5efa1a8b8f02c7abb04d.jpg 1920w, /assets/static/cody-davis-253925-unsplash.c0dad42.ce547449449f5efa1a8b8f02c7abb04d.jpg 2560w"
              data-sizes="(max-width: 2560px) 100vw, 2560px"
              class="thumbnail g-image g-image--lazy g-image--loaded"
              srcset="
                https://gridsome-forestry.netlify.app/assets/static/cody-davis-253925-unsplash.b6e36c6.ce547449449f5efa1a8b8f02c7abb04d.jpg  480w,
                https://gridsome-forestry.netlify.app/assets/static/cody-davis-253925-unsplash.1c9e94c.ce547449449f5efa1a8b8f02c7abb04d.jpg 1024w,
                https://gridsome-forestry.netlify.app/assets/static/cody-davis-253925-unsplash.f11e5e1.ce547449449f5efa1a8b8f02c7abb04d.jpg 1920w,
                https://gridsome-forestry.netlify.app/assets/static/cody-davis-253925-unsplash.c0dad42.ce547449449f5efa1a8b8f02c7abb04d.jpg 2560w
              "
              sizes="(max-width: 2560px) 100vw, 2560px"
            /><noscript data-v-50cbff3e=""
              ><img
                src="https://gridsome-forestry.netlify.app/assets/static/cody-davis-253925-unsplash.c0dad42.ce547449449f5efa1a8b8f02c7abb04d.jpg"
                class="thumbnail g-image g-image--loaded"
                width="2560"
                alt="Pineapple"
            /></noscript>
            <h3 data-v-50cbff3e="" class="project-title">Pineapple</h3>
            <div data-v-50cbff3e="" class="categories">
              <span data-v-50cbff3e="" class="category">photography</span
              ><span data-v-50cbff3e="" class="category">blue</span>
            </div></a
          >
        </div>
        <div data-v-50cbff3e="" class="project">
          <a data-v-50cbff3e="" href="/projects/3d-graff/" class="project-link"
            ><img
              data-v-50cbff3e=""
              alt="Ice Cream"
              src="https://gridsome-forestry.netlify.app/assets/static/ian-dooley-281897-unsplash.c0dad42.4ee4f858cbb8392c2cc4019598c07dcd.jpg"
              width="2560"
              data-src="https://gridsome-forestry.netlify.app/assets/static/ian-dooley-281897-unsplash.c0dad42.4ee4f858cbb8392c2cc4019598c07dcd.jpg"
              data-srcset="https://gridsome-forestry.netlify.app/assets/static/ian-dooley-281897-unsplash.b6e36c6.4ee4f858cbb8392c2cc4019598c07dcd.jpg 480w, /assets/static/ian-dooley-281897-unsplash.1c9e94c.4ee4f858cbb8392c2cc4019598c07dcd.jpg 1024w, /assets/static/ian-dooley-281897-unsplash.f11e5e1.4ee4f858cbb8392c2cc4019598c07dcd.jpg 1920w, /assets/static/ian-dooley-281897-unsplash.c0dad42.4ee4f858cbb8392c2cc4019598c07dcd.jpg 2560w"
              data-sizes="(max-width: 2560px) 100vw, 2560px"
              class="thumbnail g-image g-image--lazy g-image--loaded"
              srcset="
                https://gridsome-forestry.netlify.app/assets/static/ian-dooley-281897-unsplash.b6e36c6.4ee4f858cbb8392c2cc4019598c07dcd.jpg  480w,
                https://gridsome-forestry.netlify.app/assets/static/ian-dooley-281897-unsplash.1c9e94c.4ee4f858cbb8392c2cc4019598c07dcd.jpg 1024w,
                https://gridsome-forestry.netlify.app/assets/static/ian-dooley-281897-unsplash.f11e5e1.4ee4f858cbb8392c2cc4019598c07dcd.jpg 1920w,
                https://gridsome-forestry.netlify.app/assets/static/ian-dooley-281897-unsplash.c0dad42.4ee4f858cbb8392c2cc4019598c07dcd.jpg 2560w
              "
              sizes="(max-width: 2560px) 100vw, 2560px"
            /><noscript data-v-50cbff3e=""
              ><img
                src="https://gridsome-forestry.netlify.app/assets/static/ian-dooley-281897-unsplash.c0dad42.4ee4f858cbb8392c2cc4019598c07dcd.jpg"
                class="thumbnail g-image g-image--loaded"
                width="2560"
                alt="Ice Cream"
            /></noscript>
            <h3 data-v-50cbff3e="" class="project-title">Ice Cream</h3>
            <div data-v-50cbff3e="" class="categories">
              <span data-v-50cbff3e="" class="category">photography</span
              ><span data-v-50cbff3e="" class="category">yellow</span>
            </div></a
          >
        </div>
        <div data-v-50cbff3e="" class="project">
          <a
            data-v-50cbff3e=""
            href="/projects/ios-concept/"
            class="project-link"
            ><img
              data-v-50cbff3e=""
              alt="Porta400"
              src="https://gridsome-forestry.netlify.app/assets/static/markus-spiske-516263-unsplash.c0dad42.5fc4651133067e67284df56f3d81be2d.jpg"
              width="2560"
              data-src="https://gridsome-forestry.netlify.app/assets/static/markus-spiske-516263-unsplash.c0dad42.5fc4651133067e67284df56f3d81be2d.jpg"
              data-srcset="https://gridsome-forestry.netlify.app/assets/static/markus-spiske-516263-unsplash.b6e36c6.5fc4651133067e67284df56f3d81be2d.jpg 480w, /assets/static/markus-spiske-516263-unsplash.1c9e94c.5fc4651133067e67284df56f3d81be2d.jpg 1024w, /assets/static/markus-spiske-516263-unsplash.f11e5e1.5fc4651133067e67284df56f3d81be2d.jpg 1920w, /assets/static/markus-spiske-516263-unsplash.c0dad42.5fc4651133067e67284df56f3d81be2d.jpg 2560w"
              data-sizes="(max-width: 2560px) 100vw, 2560px"
              class="thumbnail g-image g-image--lazy g-image--loaded"
              srcset="
                https://gridsome-forestry.netlify.app/assets/static/markus-spiske-516263-unsplash.b6e36c6.5fc4651133067e67284df56f3d81be2d.jpg  480w,
                https://gridsome-forestry.netlify.app/assets/static/markus-spiske-516263-unsplash.1c9e94c.5fc4651133067e67284df56f3d81be2d.jpg 1024w,
                https://gridsome-forestry.netlify.app/assets/static/markus-spiske-516263-unsplash.f11e5e1.5fc4651133067e67284df56f3d81be2d.jpg 1920w,
                https://gridsome-forestry.netlify.app/assets/static/markus-spiske-516263-unsplash.c0dad42.5fc4651133067e67284df56f3d81be2d.jpg 2560w
              "
              sizes="(max-width: 2560px) 100vw, 2560px"
            /><noscript data-v-50cbff3e=""
              ><img
                src="https://gridsome-forestry.netlify.app/assets/static/markus-spiske-516263-unsplash.c0dad42.5fc4651133067e67284df56f3d81be2d.jpg"
                class="thumbnail g-image g-image--loaded"
                width="2560"
                alt="Porta400"
            /></noscript>
            <h3 data-v-50cbff3e="" class="project-title">Porta400</h3>
            <div data-v-50cbff3e="" class="categories">
              <span data-v-50cbff3e="" class="category">photography</span
              ><span data-v-50cbff3e="" class="category">yellow</span>
            </div></a
          >
        </div> -->
      </div>
    </div>
    <div data-v-460714ac="" >
      <div class="latest-journals-heading container" data-v-460714ac="">
        <span class="label" data-v-460714ac="">Latest and greatest</span>
      </div>
      <div class="latest-journals" data-v-460714ac="" >
        <div class="container" data-v-460714ac="">
          <a
            v-for="edge in $page.articles.edges" :key="edge.node.id"
            href="/"
            class="journal"
            data-v-460714ac=""
            ><h3 class="journal-title" data-v-460714ac="">
              {{edge.node.title}}
            </h3>
          </a>
        </div>
      </div>
    </div>
  </Layout>
</template>
<page-query>
query ($page: Int){
  posts: allStrapiPost(sortBy: "created_at", order: ASC, perPage: 10, page: $page) @paginate {
    pageInfo{
      totalPages
      currentPage
    }
    edges{
      node{
        id
        title,
        created_at,
        color,
        big_picture{
          url
        },
      }
    },
    
  }
  articles: allStrapiArticle(sortBy: "created_at", order: ASC, perPage: 10, page: $page) @paginate {
    pageInfo{
      totalPages
      currentPage
    }
    edges{
      node{
        id,
        title,
        author,
        date
      }
    },
    
  }

  general: allStrapiGeneral {
    edges {
      node {
        id 
        title 
        subtitle 
        cover {
          url
        }
      }
    }
  }
 

 
}


</page-query>

<script>
import { Pager } from "gridsome";
export default {
  metaInfo: {
    title: "Portfolio",
  },
  name: "HomePage",
  components: {
    Pager,
  },
  computed: {
    general() {
      return this.$page.general.edges[0].node;
    },
  },
  mounted() {
    console.log(this.$page.articles);
  },
};
</script>

<style>
</style>
