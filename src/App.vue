<template>
  <div class="app">

    <!-- Navbar -->
    <header class="navbar">
      <div class="logo">
        <h2>SMK Yadika Soreang</h2>
        <span>OnlineShop</span>
      </div>

      <nav>
        <RouterLink to="/">Landing</RouterLink>
        <RouterLink to="/product">Product</RouterLink>
        <RouterLink to="/about">About</RouterLink>
      </nav>
    </header>

    <!-- Isi halaman -->
    <main class="content">
      <RouterView />
    </main>

    <!-- Footer -->
    <footer>
      <p>© 2026 SMK Yadika Soreang — Onlineshop Sekolah</p>
      <p>Belanja gampang, sekolah senang.</p>
    </footer>

  </div>
</template>

<style>
/* Reset */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: Arial, Helvetica, sans-serif;
  background: #f5f7fb;
  color: #222;
}

/* Tampilan utama */
.app {
  min-height: 100vh;
  display: flex;
  flex-direction: column;
}

/* NAVBAR */
.navbar {
  background: #2563eb;
  color: white;
  padding: 18px 50px;

  display: flex;
  align-items: center;
  justify-content: space-between;

  box-shadow: 0 3px 10px rgba(0, 0, 0, 0.15);
}

.logo h2 {
  font-size: 22px;
  margin-bottom: 3px;
}

.logo span {
  font-size: 14px;
  opacity: 0.9;
}

/* MENU */
nav {
  display: flex;
  gap: 10px;
}

nav a {
  color: white;
  text-decoration: none;
  padding: 10px 16px;
  border-radius: 8px;
  transition: 0.3s;
}

nav a:hover {
  background: white;
  color: #2563eb;
}

/* Halaman aktif */
nav a.router-link-active {
  background: white;
  color: #2563eb;
}

/* CONTENT */
.content {
  flex: 1;
  padding: 50px;
  max-width: 1200px;
  width: 100%;
  margin: auto;
}

/* FOOTER */
footer {
  background: #1e293b;
  color: white;
  text-align: center;
  padding: 20px;
  margin-top: auto;
}

footer p:first-child {
  font-weight: bold;
  margin-bottom: 5px;
}

footer p:last-child {
  color: #cbd5e1;
  font-size: 14px;
}

/* Responsive HP */
@media (max-width: 700px) {
  .navbar {
    flex-direction: column;
    gap: 15px;
    padding: 20px;
  }

  nav {
    flex-wrap: wrap;
    justify-content: center;
  }

  .content {
    padding: 25px;
  }
}
</style>