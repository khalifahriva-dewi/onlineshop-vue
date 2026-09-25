<template>
  <main>
    <section class="hero">
      <h1>
        Belanja Perlengkapan Sekolah,
        Gampang & Terpercaya
      </h1>
      <p>
        Dari kaos, topi, sampai tas sekolah —
        semua ada di satu tempat.
      </p>
      <a href="#produk" class="btn">
        Lihat Produk
      </a>
    </section>

    <video controls width="480" muted loop>
      <source src="/video/mov_bbb (1).mp4" type="video/mp4" />
      Browser kamu tidak mendukung pemutaran video.
    </video>

    <section class="features" id="produk">
      <div class="feature-card">
        <div class="icon">
          ✓
        </div>
        <h3>
          Kualitas Terjamin
        </h3>
        <p>
          Bahan dengan kualitas yang
          sudah terpilih.
        </p>
      </div>

      <div class="feature-card">
        <div class="icon">
          💰
        </div>
        <h3>
          Harga Bersahabat
        </h3>
        <p>
          Harga ramah di kantong
          semua siswa.
        </p>
      </div>


      <div class="feature-card">
        <div class="icon">
          🏫
        </div>
        <h3>
          Ambil di Sekolah
        </h3>
        <p>
          Tidak perlu ongkir,
          ambil di koperasi.
        </p>
      </div>
    </section>
  </main>
</template>


<style scoped>
* {
  box-sizing: border-box;
}
main {
  min-height: 100vh;
  background: #f8fbff;
  padding-bottom: 50px;
}
.hero {
  width: 90%;
  max-width: 1000px;
  min-height: 300px;
  margin: 30px auto;
  padding: 50px 20px;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  text-align: center;
  background: linear-gradient(
    110deg,
    #4c63e9,
    #6635ee
  );
  border-radius: 2px;
  color: white;
}

.hero h1 {
  margin: 0 0 15px;
  max-width: 700px;
  font-family: Georgia, "Times New Roman", serif;
  font-size: 32px;
  line-height: 1.2;
  color: white;
}

.hero p {
  margin: 0 0 25px;
  color: #e5e5ff;
  font-size: 14px;
}

.btn {
  display: inline-block;
  padding: 12px 25px;
  background: white;
  color: #5146dc;
  text-decoration: none;
  font-size: 14px;
  font-weight: bold;
  border-radius: 25px;
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.15);
  transition: 0.3s;
}

.btn:hover {
  transform: translateY(-2px);
  box-shadow:
    0 6px 18px rgba(0, 0, 0, 0.2);
}

video {
  display: block;
  width: 480px;
  max-width: 90%;
  margin: 30px auto;
  border-radius: 10px;
  box-shadow:
    0 5px 20px rgba(0, 0, 0, 0.12);
}

.features {
  width: 90%;
  max-width: 850px;
  margin: 35px auto;
  display: flex;
  justify-content: center;
  align-items: flex-start;
  flex-wrap: wrap;
  gap: 0;
}

.feature-card {
  width: 280px;
  min-height: 120px;
  padding: 20px;
  background: white;
  text-align: center;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  box-shadow:
    0 4px 15px rgba(0, 0, 0, 0.08);
  border-radius: 4px;
}

.icon {
  font-size: 25px;
  margin-bottom: 8px;
}

.feature-card h3 {
  margin: 0 0 7px;
  font-size: 15px;
  color: #222;
}

.feature-card p {
  margin: 0;
  max-width: 200px;
  color: #888;
  font-size: 11px;
  line-height: 1.4;
}

@media (max-width: 700px) {
  .hero {
    width: 95%;
    min-height: 280px;
    padding: 35px 15px;
  }
  .hero h1 {
    font-size: 25px;
  }
  .hero p {
    font-size: 13px;
  }
  .features {
    flex-direction: column;
    align-items: center;
    gap: 15px;
  }
  .feature-card {
    width: 100%;
    max-width: 350px;
  }
  video {
    width: 90%;
  }
}
</style>