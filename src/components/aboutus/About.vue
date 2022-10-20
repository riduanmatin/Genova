<!-- eslint-disable vue/multi-word-component-names -->
<template>
  <section class="container mx-auto">
    <div class="container-awal">
      <div class="about-section">
        <div class="inner-container inner-container-shadow">
          <h1>About Us</h1>
          <p class="font-semibold">
            GENOVA adalah perusahaan yang bergerak memproduksi Premium Sirup,
            Powder Drink dan Fruitblend dengan harga yang terjangkau.
            Menggunakan bahan baku impor berkualitas, bersertifikasi halal serta
            diproduksi di Jakarta, Indonesia.Sehingga ketersediaan stock untuk
            pasokan bahan baku minuman selalu terjaga.<br /><br />

            Produk Genova juga sudah memiliki sertifikat BPOM di beberapa produk
            unggulan dan terus mengupdate semua produknya agar memiliki
            sertifikat BPOM. Sehingga produk kami aman untuk digunakan sebagai
            bahan baku minuman<br /><br />

            GENOVA saat ini sudah dipercaya oleh lebih dari 1000 pelanggan setia
            dari hotel bintang lima maupun cafe papan atas di seluruh
            Indonesia.<br /><br />

            Product GENOVA banyak digunakan untuk campuran pembuatan mocktail,
            cocktail, milkshake, ice blend, hot drink dan lain-lain. Tersedia
            dalam ragam varian rasa.<br /><br />
          </p>
          <div class="skills">
            <span>Web Design</span>
            <span>Photoshop & Illustrator</span>
            <span>Coding</span>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
.container-awa {
  min-height: 100vh;
  display: flex;
  align-items: center;
  justify-content: center;
  background-color: #f1f1f1;
}
.about-section {
  background: url(../../assets/images/syrup_bubble_gum-removebg-preview.png)
    no-repeat left;
  background-size: contain;
  background-position: center center;
  background-color: #fdfdfd;
  overflow: hidden;
  padding: 100px 0;
}

.inner-container {
  width: 55%;
  float: right;
  background-color: #fdfdfd;
  padding: 45px;
}

.inner-container-shadow {
  box-shadow: rgba(6, 24, 44, 0.4) 0px 0px 0px 2px,
    rgba(6, 24, 44, 0.65) 0px 4px 6px -1px,
    rgba(255, 255, 255, 0.08) 0px 1px 0px inset;
}

.inner-container h1 {
  margin-bottom: 30px;
  font-size: 30px;
  font-weight: 900;
}

@media screen and (max-width: 1200px) {
  .inner-container {
    padding: 80px;
  }
}

@media screen and (max-width: 1000px) {
  .about-section {
    background-size: 100%;
    padding: 100px 40px;
  }
  .inner-container {
    width: 100%;
  }
}

@media screen and (max-width: 600px) {
  .about-section {
    padding: 0;
  }
  .inner-container {
    padding: 60px;
  }
}
</style>
