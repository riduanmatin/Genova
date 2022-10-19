<!-- eslint-disable vue/multi-word-component-names -->
<template>
  <section class="container mx-auto">
    <div class="flex flex-col gap-6 py-6 px-4 lg:px-6 lg:py-12 xl:px-12">
      <div class="contact-info">
        <div class="card">
          <i class="card-icon far fa-envelope"></i>
          <p>email@domain.com</p>
        </div>

        <div class="card">
          <i class="card-icon fas fa-phone"></i>
          <p>+000000000000</p>
        </div>

        <div class="card">
          <i class="card-icon fas fa-map-marker-alt"></i>
          <p>New York, USA</p>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
.contact-info {
  display: flex;
  width: 100%;
  max-width: 1200px;
  align-items: center;
  justify-content: center;
  padding: 0 20px;
}

.card {
  background: #2f3542;
  padding: 0 20px;
  margin: 0 10px;
  width: calc(33% - 20px);
  height: 200px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  color: #fff;
  cursor: pointer;
}

.card-icon {
  font-size: 28px;
  background: #ff6348;
  width: 60px;
  height: 60px;
  text-align: center;
  line-height: 60px !important;
  border-radius: 50%;
  transition: 0.3s linear;
}

.card:hover .card-icon {
  background: none;
  color: #ff6348;
  transform: scale(1.6);
}

.card p {
  margin-top: 20px;
  font-weight: 300;
  letter-spacing: 2px;
  max-height: 0;
  opacity: 0;
  transition: 0.3s linear;
}

.card:hover p {
  max-height: 40px;
  opacity: 1;
}

@media screen and (max-width: 800px) {
  .contact-info {
    flex-direction: column;
  }
  .card {
    width: 100%;
    max-width: 300px;
    margin: 10px 0;
  }
}
</style>
