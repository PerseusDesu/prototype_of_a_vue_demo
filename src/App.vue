<template>
  <div id="app">
    <div class="head">    
      <the-head></the-head>
    </div>
    <div class="mid">
      <div class="side">
        <the-side></the-side>
      </div>
      <div class="main">
        <the-main></the-main>
        <div class="lists">
          <the-lists></the-lists>
        </div>
      </div>
    </div>
    <div class="footer">
      <the-footer></the-footer>
    </div>

  </div>
</template>

<script>
import TheHead from './components/TheHead/index.vue'
import TheSide from './components/TheSide/index.vue'
import TheMain from './components/TheMain/index.vue'
import TheLists from './components/TheLists/index.vue'
import TheFooter from './components/TheFooter/index.vue'

export default {
  name: 'App',
  components: {
    TheHead,
    TheSide,
    TheMain,
    TheLists,
    TheFooter
  }
}
</script>

<style>
.side{
  width: 500px;
}

.lists{
  margin-left: 240px;
}

.footer{
  margin-top: 150px;
  margin-left: 560px;
}
</style>
