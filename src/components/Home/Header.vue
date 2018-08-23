<template>
  <header>
    <nav class="navbar navbar-expand-lg navbar-light menu-top">
      <span class="navbar-brand d-block text-center">
        <a href="#" class="brand-name">Duc Pham</a>
        <div class="brand-small">Javascript developer</div>
      </span>

      <div id="navbarTogglerDemo03">
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
export default {}
</script>

<style lang="scss">
$textColor: #4D4D4D;

.menu-top {
  margin-left: calc((100% - 980px) / 2);
  width: 980px;
  .navbar-brand {
    text-align: center;
    padding: 60px 0;
    .brand-name {
      color: $textColor;
      text-decoration: none;
      font-size: 38px;
      font-weight: bold;
    }
    .brand-small {
      color: $textColor
    }
  }
  .navbar-nav {
    .active {
      a {
        color: #61d0d4 !important;
      }
    }
    .nav-item {
     .nav-link {
        text-transform: uppercase;
        font-weight: 600;
     }
      &:hover {
        a {
          color: #61d0d4;
        }
      }
    }
  }
}

#navbarTogglerDemo03 {
  margin-top: 45px;
    margin-left: 10px;
}

@media (max-width: 576px) {
  #navbarTogglerDemo03 {
    display: none;
  }
  .navbar-brand {
    padding: 20px 10px;
    width: 100%;
  }
  .menu-top {
    width: 100%;
    margin-left: 0;
    .brand-name {
      font-size: 18px;
    }
    .navbar-nav {
      visibility: hidden;
    }
  }
}
</style>
