<script setup>
import ProductCard from '../components/ProductCard.vue'

const daftarProduk = [
  {
    id: 1,
    nama: 'Seragam Sekolah',
    harga: 150000,
    gambar: 'https://placehold.co/150'
  },
  {
    id: 2,
    nama: 'Topi Sekolah',
    harga: 35000,
    gambar: 'https://placehold.co/150'
  },
  {
    id: 3,
    nama: 'Tas Sekolah',
    harga: 120000,
    gambar: 'https://placehold.co/150'
  }
]
</script>

<template>
  <main>
    <h1>Produk Kami</h1>

    <div class="grid">
      <ProductCard
        v-for="produk in daftarProduk"
        :key="produk.id"
        :nama="produk.nama"
        :harga="produk.harga"
        :gambar="produk.gambar"
      />
    </div>
  </main>
</template>

<style scoped>
main {
  padding: 30px 50px;
}

h1 {
  margin-bottom: 20px;
}

.grid {
  display: flex;
  gap: 20px;
  flex-wrap: wrap;
}
</style>