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
        <NuxtLink style="text-decoration: none" to="/dashboard"><b-nav-item class="nav-item" to="/dashboard" active>Dashboard</b-nav-item></NuxtLink>
        <b-nav-item class="nav-item" to="/dashboard#sec2">Jadwal</b-nav-item>
        <b-nav-item class="nav-item" to="/">Bantuan</b-nav-item>
      </b-navbar-nav>
    <b-dropdown id="dropdown-right" right text="mrezkys" variant="outline-light" class="m-2">
        <b-dropdown-item to="/dashboard/profile">Profil</b-dropdown-item>
        <b-dropdown-item to="/">Keluar</b-dropdown-item>
    </b-dropdown>
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

  .user-profile{
      height: 100%;
      width: 240px;
      background-color: black;
  }

  .user-profile .user-avatar{
      width: 42px;
      height: 42px;
      border-radius: 100%;
      background-color: grey;
  }
</style>