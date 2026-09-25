<script setup>
defineProps({
  nama: String,
  harga: Number,
  gambar: String
})

function masukkanKeranjang() {
  alert('Produk berhasil dimasukkan ke keranjang!')
}

function beli() {
  alert('Produk siap dibeli!')
}
</script>

<template>
  <div class="card">
    <img :src="gambar" :alt="nama">

    <h3>{{ nama }}</h3>

    <p>Rp {{ harga }}</p>

    <button @click="masukkanKeranjang">
      Masukkan Keranjang
    </button>

    <button @click="beli">
      Beli
    </button>
  </div>
</template>

<style scoped>
.card {
  width: 220px;
  border: 1px solid #ddd;
  padding: 20px;
  border-radius: 15px;
  text-align: center;
  background: white;
  box-shadow: 0 4px 10px rgba(0, 0, 0, 0.08);
  transition: 0.3s;
}

.card:hover {
  transform: translateY(-5px);
  box-shadow: 0 8px 18px rgba(0, 0, 0, 0.15);
}

.card img {
  width: 150px;
  height: 150px;
  object-fit: cover;
  border-radius: 10px;
}

.card h3 {
  margin: 12px 0 8px;
  color: #333;
}

.card p {
  font-weight: bold;
  color: #2563eb;
  font-size: 18px;
}

/* Tombol */
button {
  padding: 10px 14px;
  margin: 5px 3px;
  border: none;
  border-radius: 8px;
  cursor: pointer;
  font-weight: bold;
  transition: 0.2s;
}

/* Tombol keranjang */
button:first-of-type {
  background: #f1f5f9;
  color: #2563eb;
  border: 1px solid #2563eb;
}

button:first-of-type:hover {
  background: #2563eb;
  color: white;
}

/* Tombol beli */
button:last-of-type {
  background: #2563eb;
  color: white;
}

button:last-of-type:hover {
  background: #1d4ed8;
  transform: scale(1.05);
}
</style>