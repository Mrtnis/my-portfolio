<template>
  <section class="home px-3">
    <!-- card-profil -->
    <div class="row pt-3 pb-3">
      <div class="col-md-5">
        <Profil />
      </div>
    </div>
  </section>
</template>

<script>
import Profil from './Profil.vue';

export default {
  components: {
    Profil,
  },
};
</script>

<style scoped>
.home {
  background-color: var(--secondary-color);
  border-radius: var(--border-primary);
  min-height: 50vh;
}
</style>
