
<script setup>
</script>


<template>
      <nav class="navbar bg-danger-subtle navbar-expand-lg">
    <div class="container-fluid">
      <a class="navbar-brand" href="#" >
      <img class="logo" src="@/assets/logoile.png" alt="Logo"/>
      </a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarNav">
        <ul class="navbar-nav justify-content-end">
          <li class="nav-item">
            <a class="nav-link active" aria-current="page" href="#">Home</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#PortfolioItem">Portfolio</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#Footer">Contatti</a>
          </li>
        </ul>
      </div>
    </div>
  </nav>
</template>

<style scoped>
.logo {
  position: static;
  width: 100px;
  height: 100px;
}
</style>
