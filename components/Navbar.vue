<template>
<div>
  <b-navbar toggleable="lg" type="dark" variant="dark" class="navbar p-0 bg-transparent">
    <b-navbar-brand to="/" >
      <img  src="~assets/icons/logo.svg" alt="">
      <h5 class="company-name d-inline">Healthconf</h5>
    </b-navbar-brand>
    <b-navbar-toggle target="nav-text-collapse"></b-navbar-toggle>
    <b-collapse id="nav-text-collapse" is-nav>
      <b-navbar-nav class="mr-auto">
        <b-nav-item class="nav-item" to="/" nuxt-link-active='/relawan'>Home</b-nav-item>
        <b-nav-item class="nav-item" to="/relawan">Relawan</b-nav-item>
        <b-nav-item class="nav-item" to="/program">Program</b-nav-item>
        <b-nav-item class="nav-item" to="/tentang-kami">Tentang Kami</b-nav-item>
      </b-navbar-nav>
      <b-navbar-nav>
        <b-nav-item class="nav-item" to="/auth">Masuk</b-nav-item>
      </b-navbar-nav>
    </b-collapse>
  </b-navbar>
</div>
</template>

<style scoped>
  .navbar{
    padding: 20px 0 !important;
  }

  .navbar .company-name{
      margin: 0 15px;
      font-family: 'Visby CF';
      font-weight: 700;
      font-size: 22px;
  }
</style>