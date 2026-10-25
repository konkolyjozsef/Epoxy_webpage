<script setup>
import Welcome from '../pages/Welcome.vue'
</script>

<template>
  <header class="epoxy-bg">
    <nav class="navbar navbar-expand-lg py-3 " >
      <div class="container">
        <a class="navbar-brand fw-bold" href="/">
          EPOXY LOGO
        </a>

        <!-- Hamburgergomb mobilra -->
        <button
          class="navbar-toggler"
          type="button"
          data-bs-toggle="collapse"
          data-bs-target="#epoxyMenu"
        >
          <span class="navbar-toggler-icon"><i class="fa-solid fa-bars"></i></span>
        </button>

        <!-- Lenyíló menü -->
        <div id="epoxyMenu" class="collapse navbar-collapse">
          <ul class="navbar-nav ms-auto gap-lg-4 pt-3 pt-lg-0">
            <li class="nav-item">
              <a class="nav-link" href="#alkotasok">
                Alkotások
              </a>
            </li>

            <li class="nav-item">
              <a class="nav-link" href="#rolam">
                Rólam
              </a>
            </li>

            <li class="nav-item order">
              <a class="nav-link" href="#egyedi-rendeles">
                Egyedi rendelés
              </a>
            </li>
          </ul>
        </div>
      </div>
    </nav>
  </header>

  <main>
    <slot />
  </main>

  <footer class="container">
    <div class="footer">
      <div class="row">
        <div class="col-12 col-md-4 col-lg-4 py-5">
          <h2>
            Epoxy műhely
          </h2>

          <p>
            Kézzel készült epoxy tárgyak.
          </p>
        </div>
        <div class="col-12 col-md-4 col-lg-4 py-5 footer-divider">
          <h2>Fedezd fel</h2>
          az oldalakat
        </div>
        <div class="col-12 col-md-4 col-lg-4 py-5 footer-divider">
          <h2>Kapcsolat</h2>
          <span>
            <i class="fa-solid fa-envelope"></i> info@epoxy.hu
          </span>
        </div>

      </div>
    </div>
    <div class="socket mt-2">
      <p class="text-center mt-3">
        &copy; 2026 Epoxy. Minden jog fenntartva.
      </p>
    </div>
  </footer>
</template>
<style scoped>
</style>
