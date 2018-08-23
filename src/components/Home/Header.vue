<template>
  <header>
    <nav class="navbar navbar-expand-lg navbar-light menu-top">
      <button class="navbar-toggler float-right" type="button" data-toggle="collapse" data-target="#navbarTogglerDemo03" aria-controls="navbarTogglerDemo03" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <span class="navbar-brand">
        <a href="#" class="brand-name">Duc Pham</a>
        <div class="brand-small">JavaScript Development</div>
      </span>

      <div class="collapse navbar-collapse" id="navbarTogglerDemo03">
        <ul class="navbar-nav mr-auto mt-2 mt-lg-0">
          <li class="nav-item active">
            <router-link class="nav-link" to="/">Home
              <span class="sr-only">(current)</span>
            </router-link>
          </li>
          <li class="nav-item">
            <router-link to="resume" class="nav-link">Resume</router-link>
          </li>
          <li class="nav-item">
            <router-link to="project" class="nav-link">Project</router-link>
          </li>
          <li class="nav-item">
            <router-link to="contact" class="nav-link">Contact</router-link>
          </li>
        </ul>
      </div>
    </nav>
  </header>

</template>

<script>
export default {

}
</script>

<style lang="scss">
.menu-top {
  margin-left: calc((100% - 980px) / 2);
  width: 980px;
  .navbar-brand {
    text-align: center;
    .brand-name {
      color: rgba(0, 0, 0, 0.9);
      font-size: 38px;
      font-weight: bold;
    }
  }
  .navbar-nav {
    text-transform: uppercase;
    .active {
      a {
        color: #61d0d4 !important;
      }
    }
    .nav-item {
      &:hover {
        a {
          color: #61d0d4;
        }
      }
    }
  }
}

@media (max-width: 576px) {
  .menu-top {
    width: 100%;
    margin-left: 0;
    .brand-name {
      font-size: 18px;
    }
    .navbar-nav {
      text-align: center;
      a {
        border: 1px dashed #cfcfcf;
      }
    }
  }
}
</style>
