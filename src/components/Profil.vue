<template>
  <div class="card-profil">
    <div class="profil-bg">
      <div class="profil-photo">M</div>
    </div>
    <div class="my-name mt-4 fw-bold">Martunis</div>
    <div class="my-title"><i class="bi bi-laptop me-1"></i> Front End Developer</div>
    <div class="my-title"><i class="bi bi-phone me-1"></i> Mobile Developer</div>
    <div class="my-title"><i class="bi bi-geo-fill me-1"></i> Aceh</div>
    <div class="row mt-3">
      <div class="col-md-6 wrap-contact" v-for="contact in dataContact" :key="contact.id">
        <div class="my-contact">
          <i :class="contact.icon"></i>
          <div>{{ contact.name }}</div>
          <div>{{ contact.value }}</div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      dataContact: [
        {
          id: 1,
          icon: 'bi bi-envelope',
          name: 'email',
          value: 'nis210698@gmail.com',
        },
        {
          id: 2,
          icon: 'bi bi-whatsapp',
          name: 'whatsapp',
          value: '+62 822 9861 5112',
        },
      ],
    };
  },
};
</script>

<style scoped>
.card-profil {
  background-color: #fff;
  border-radius: 10px;
  padding: 10px;
}
.profil-bg {
  height: 120px;
  border-radius: 10px;
  background-color: var(--third-color);
  position: relative;
}
.profil-photo {
  width: 50px;
  height: 50px;
  border-radius: 10px;
  background-color: var(--third-color);
  position: absolute;
  left: 15px;
  bottom: -20px;
  box-shadow: 0 0 0 2px #fff;
  line-height: 50px;
  text-align: center;
  color: #fff;
  font-weight: 700;
  font-size: 23px;
}
.my-name,
.my-title {
  margin-left: 15px;
}
.my-title {
  font-size: 12px;
}
.my-contact {
  width: 100%;
  padding: 10px;
  background-color: var(--secondary-color);
  border-radius: 10px;
  font-size: 10px;
}
</style>
