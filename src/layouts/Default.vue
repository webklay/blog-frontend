<template>
  <div class="layout sticky-header" id="app">
    <!-- Navigation-->

    <header data-v-7e33895e="" class="header sticky">
      <div data-v-7e33895e class="container">
        <div data-v-7e33895e class="left">
          <a
            data-v-7e33895e
            href="/"
            aria-current="page"
            class="home-link active--exact active"
            ><img
              data-v-7e33895e
              src="http://113.31.118.228:1337/uploads/logo_332701b7_2b8b1dad2b.svg"
              alt="Nichlas W. Andersen"
              class="logo"
          /></a>
        </div>
        <nav data-v-7e33895e class="nav right">
          <a data-v-7e33895e href="/" class="nav__link">Journal</a
          ><a data-v-7e33895e href="/" class="nav__link">Say Hi!</a>
        </nav>
      </div>
    </header>
    <!-- 子组件出口  默认插槽-->
    <slot />
    <!-- Footer-->
    <footer class="footer" data-v-07acb5f8>
      <div class="container" data-v-07acb5f8>
        <span data-v-07acb5f8>Copyright © 2021</span>
      </div>
    </footer>
  </div>
</template>



<style>
</style>
