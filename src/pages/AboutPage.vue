<template>
  <section class="about-page">

    <!-- Judul -->
    <div class="about-header">
      <span class="badge">🏫 TENTANG KAMI</span>

      <h1>Tentang <span>Onlineshop Sekolah</span></h1>

      <p>
        Kenali lebih dekat Onlineshop SMK Yadika Soreang,
        tempat belanja kebutuhan sekolah dengan mudah dan nyaman.
      </p>
    </div>

    <!-- Isi About -->
    <div class="about-content">

      <!-- Card Sekolah -->
      <div class="about-card">
        <div class="icon">🏫</div>

        <h2>SMK Yadika Soreang</h2>

        <p>
          SMK Yadika Soreang merupakan sekolah yang berfokus
          pada pendidikan vokasi dan pengembangan keterampilan
          siswa agar siap menghadapi dunia kerja maupun melanjutkan
          pendidikan.
        </p>
      </div>

      <!-- Card Onlineshop -->
      <div class="about-card">
        <div class="icon">🛒</div>

        <h2>Onlineshop Sekolah</h2>

        <p>
          Onlineshop Sekolah dibuat untuk memudahkan siswa dan
          warga sekolah dalam membeli berbagai kebutuhan sekolah,
          seperti pakaian, atribut, dan perlengkapan lainnya.
        </p>
      </div>

      <!-- Card Tujuan -->
      <div class="about-card">
        <div class="icon">🎯</div>

        <h2>Tujuan Kami</h2>

        <p>
          Memberikan pengalaman belanja yang mudah, cepat,
          praktis, dan nyaman bagi seluruh warga sekolah.
        </p>
      </div>

    </div>

    <!-- Keunggulan -->
    <div class="keunggulan">

      <h2>Kenapa Belanja di Sini?</h2>

      <div class="features">

        <div class="feature">
          <div class="feature-icon">⚡</div>
          <h3>Praktis</h3>
          <p>
            Pesan kebutuhan sekolah tanpa harus datang langsung.
          </p>
        </div>

        <div class="feature">
          <div class="feature-icon">💰</div>
          <h3>Harga Terjangkau</h3>
          <p>
            Produk sekolah dengan harga yang ramah untuk siswa.
          </p>
        </div>

        <div class="feature">
          <div class="feature-icon">📦</div>
          <h3>Produk Berkualitas</h3>
          <p>
            Menyediakan produk sekolah yang nyaman dan berkualitas.
          </p>
        </div>

        <div class="feature">
          <div class="feature-icon">😊</div>
          <h3>Mudah Digunakan</h3>
          <p>
            Tampilan sederhana sehingga mudah digunakan semua orang.
          </p>
        </div>

      </div>

    </div>

  </section>
</template>

<style scoped>
/* HALAMAN ABOUT */
.about-page {
  padding: 20px 0 50px;
}

/* HEADER */
.about-header {
  text-align: center;
  max-width: 750px;
  margin: 0 auto 45px;
}

.badge {
  display: inline-block;
  background: #dbeafe;
  color: #2563eb;
  padding: 8px 16px;
  border-radius: 20px;
  font-size: 13px;
  font-weight: bold;
  margin-bottom: 15px;
}

.about-header h1 {
  font-size: 40px;
  color: #1e293b;
  margin-bottom: 15px;
}

.about-header h1 span {
  color: #2563eb;
}

.about-header p {
  color: #64748b;
  font-size: 17px;
  line-height: 1.6;
}

/* CARD ABOUT */
.about-content {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 25px;
}

.about-card {
  background: white;
  padding: 30px;
  border-radius: 18px;
  text-align: center;

  box-shadow: 0 5px 20px rgba(0, 0, 0, 0.08);

  transition: 0.3s;
}

.about-card:hover {
  transform: translateY(-8px);
  box-shadow: 0 10px 25px rgba(0, 0, 0, 0.12);
}

.icon {
  width: 70px;
  height: 70px;
  margin: 0 auto 20px;

  background: #dbeafe;
  border-radius: 50%;

  display: flex;
  justify-content: center;
  align-items: center;

  font-size: 32px;
}

.about-card h2 {
  color: #1e293b;
  margin-bottom: 12px;
}

.about-card p {
  color: #64748b;
  line-height: 1.6;
}

/* KEUNGGULAN */
.keunggulan {
  margin-top: 50px;
  background: white;
  padding: 35px;
  border-radius: 20px;
  box-shadow: 0 5px 20px rgba(0, 0, 0, 0.08);
}

.keunggulan > h2 {
  text-align: center;
  color: #1e293b;
  margin-bottom: 30px;
  font-size: 28px;
}

/* FEATURES */
.features {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 20px;
}

.feature {
  text-align: center;
  padding: 20px;
}

.feature-icon {
  font-size: 35px;
  margin-bottom: 12px;
}

.feature h3 {
  color: #2563eb;
  margin-bottom: 8px;
}

.feature p {
  color: #64748b;
  font-size: 14px;
  line-height: 1.5;
}

/* RESPONSIVE */
@media (max-width: 900px) {
  .about-content {
    grid-template-columns: 1fr;
  }

  .features {
    grid-template-columns: repeat(2, 1fr);
  }
}

@media (max-width: 600px) {
  .about-header h1 {
    font-size: 30px;
  }

  .features {
    grid-template-columns: 1fr;
  }

  .keunggulan {
    padding: 25px 15px;
  }
}
</style>