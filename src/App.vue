<template>
  <div id="app">
    <Header />
    <div class="main-content">
      <router-view/>
    </div>
  </div>
</template>

<script>
import Header from '@/components/Home/Header'
export default {
  name: 'app',
  components: {
    Header
  }
}
</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css?family=Lato:300,400,400i,700,700i,900|Roboto:100i,300,300i,400,400i,500,500i,700,700i,900&subset=vietnamese');
#app {
  font-family: 'Lato', sans-serif;
  background: #eae5e5;
  min-height: 100vh;
  .main-content {
    margin-left: calc((100% - 980px) / 2);
    width: 980px;
  }
}

@media (max-width: 576px) {
  #app {
    .main-content {
      width: 100%;
      margin-left: 0;
    }
  }
}
</style>
