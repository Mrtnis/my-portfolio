<template>
  <section class="jobs">
    <div class="card-title">Work Experience</div>
    <div class="card-body mb-3" v-for="office in officeWork" :key="office.id">
      <div class="row">
        <div class="col-md-4 wrap-img mb-2">
          <div class="row px-2">
            <div class="circle m-auto">{{ office.avaName }}</div>
          </div>
        </div>
        <div class="col-md-8">
          <div class="row mb-2">
            <b>{{ office.name }}</b>
          </div>
          <div class="row mb-2">
            <div class="col-auto from"><i class="bi bi-calendar-minus me-1"></i> {{ office.startDate }}</div>
            <div class="col-auto to"><i class="bi bi-calendar-check me-1"></i> {{ office.endDate }}</div>
          </div>
          <div class="row">
            <div class="col-md">
              <div class="position">{{ office.position }}</div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      officeWork: [
        {
          id: 1,
          name: 'CV Juang Andalan Teknologi',
          avaName: 'J',
          position: 'Junior Programmer',
          startDate: '25-02-2021',
          endDate: '25-05-2021',
        },
        {
          id: 2,
          name: 'PT Rangkai Utama Berjaya',
          avaName: 'R',
          position: 'Front End Developer',
          startDate: '03-06-2021',
          endDate: 'Now',
        },
      ],
    };
  },
};
</script>

<style scoped>
.card-body {
  border-radius: var(--border-primary);
  background-color: var(--secondary-color);
  box-shadow: 0 0 6px #dee2e6;
}
.wrap-img {
  display: flex;
  justify-content: center;
  align-items: center;
}
.circle {
  width: 75px;
  height: 75px;
  line-height: 75px;
  text-align: center;
  color: #fff;
  font-size: 30px;
  font-weight: bolder;
  border-radius: 50%;
  background-color: var(--third-color);
  border: 3px solid var(--secondary-color);
  box-shadow: 0 0 0 2px var(--third-color);
}
.from,
.to {
  font-size: 15px;
}
.position {
  font-size: 15px;
  text-align: center;
  background-color: var(--third-color);
  border-radius: 8px;
  padding: 3px;
  color: #fff;
}

@media only screen and (max-width: 600px) {
  .card-body {
    text-align: center;
  }
}
</style>
