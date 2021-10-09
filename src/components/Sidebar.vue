<template>
  <section class="sidebar">
    <div class="title mb-3"><b>Hello,</b> Everyone 👋</div>
    <div class="subtitle">Lorem ipsum dolor sit amet consectetur adipisicing elit. Eaque, fugit.</div>

    <div class="card-jobs mt-5">
      <Jobs />
    </div>
  </section>
</template>

<script>
import Jobs from './Jobs.vue';

export default {
  components: {
    Jobs,
  },
};
</script>

<style scoped>
.title {
  font-size: 25px;
}
</style>
