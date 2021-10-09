<template>
  <section class="home">
    <div class="mx-5 mt-5">
      <div class="row">
        <div class="col-md-4">
          <Sidebar />
        </div>
        <div class="col-md-8">
          <Home />
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import Sidebar from './components/Sidebar.vue';
import Home from './components/Home.vue';

export default {
  components: {
    Sidebar,
    Home,
  },
};
</script>

<style>
* {
  font-family: 'Roboto', sans-serif;
  --secondary-color: #f8f9fa;
  --third-color: #6fd08c;
  --border-primary: 20px;
}
.card-title {
  font-size: 18px;
  font-weight: 700;
}
</style>
