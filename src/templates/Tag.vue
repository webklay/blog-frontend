<template>
    <Layout>
   
    <!-- Page Header-->
    <header
      class="masthead"
      style="background-image: url('/img/home-bg.jpg')"
    >
      <div class="overlay"></div>
      <div class="container">
        <div class="row">
          <div class="col-lg-8 col-md-10 mx-auto">
            <div class="site-heading">
              <h1># {{$page.tag.title}}</h1>
            </div>
          </div>
        </div>
      </div>
    </header>
    <!-- Main Content-->
    <div class="container">
      <div class="row">
        <div class="col-lg-8 col-md-10 mx-auto">
          <div class="post-preview" v-for="post in $page.tag.posts" :key="post.id">
            <g-link :to="'/post/' + post.id">
              <h2 class="post-title">
                {{post.title}}
              </h2>
              <!-- <h3 class="post-subtitle">
                Problems look mighty small from 150 miles up
              </h3> -->
            </g-link>
            <p class="post-meta">
              Posted by
              <a href="#!">joy</a>
              on {{post.created_at}}
            </p>
            <p>
              <span v-for="tag in post.tags" :key="tag.id">
                <g-link :to="'/tag/' + tag.id" >{{tag.title}}</g-link>
                &nbsp;&nbsp;
              </span>
            </p>
            <hr />
          </div>
          <!-- <hr /> -->
          <!-- <div class="post-preview">
            <a href="post.html"
              ><h2 class="post-title">
                I believe every human has a finite number of heartbeats. I don't
                intend to waste any of mine.
              </h2></a
            >
            <p class="post-meta">
              Posted by
              <a href="#!">Start Bootstrap</a>
              on September 18, 2021
            </p>
          </div>
          <hr />
          <div class="post-preview">
            <a href="post.html">
              <h2 class="post-title">Science has not yet mastered prophecy</h2>
              <h3 class="post-subtitle">
                We predict too much for the next year and yet far too little for
                the next ten.
              </h3>
            </a>
            <p class="post-meta">
              Posted by
              <a href="#!">Start Bootstrap</a>
              on August 24, 2021
            </p>
          </div>
          <hr />
          <div class="post-preview">
            <a href="post.html">
              <h2 class="post-title">Failure is not an option</h2>
              <h3 class="post-subtitle">
                Many say exploration is part of our destiny, but it’s actually
                our duty to future generations.
              </h3>
            </a>
            <p class="post-meta">
              Posted by
              <a href="#!">Start Bootstrap</a>
              on July 8, 2021
            </p>
          </div>
          <hr /> -->
          <!-- Pager-->
          <!-- <div class="clearfix">
            <a class="btn btn-primary float-right" href="#!">Older Posts →</a>
          </div> -->

        </div>
      </div>
    </div>
  
  </Layout>
</template>

<page-query>
query($id: ID!){
   tag: strapiTag(id: $id){
        id 
        title 
        posts {
            id 
            title
        }
    }
}

</page-query>
<script>
    export default {
        name: 'TagPage'
    }
</script>

<style scoped>

</style>