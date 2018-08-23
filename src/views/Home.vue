<template>
  <div class="home container">
    <div class="row">
      <div class="col-sm-6 text-center">
        <figure class="figure">
          <img src="../assets/images/profile.jpg" class="figure-img img-fluid" alt="A generic square placeholder image with rounded corners in a figure.">
        </figure>
      </div>
      <div class="col-sm-6">
        <h1 class="text-center text-sm-left font-weight-bold">Hello,</h1>
        <h3 class="text-center text-sm-left">a bit about me:</h3>
        <div class="d-flex flex-row justify-content-between mt-3 navigation-main">
          <a href="" class="nav-main-item pink-color">My resume</a>
          <a href="" class="nav-main-item cloud-color">My work</a>
          <a href="" class="nav-main-item sticky-rice-color">My skills</a>
        </div>
        <p class="mt-4">I'm a 2+ years experienced web - mobile developer with extensive experience in building high quality sites, applications. I like working on projects with a team that cares about creating beautiful and usable interfaces. It's important to me to build long term relationships with clients, so I'm primarily looking for long term projects. I'm flexible with my working hours and am happy to work closely with any existing freelancers you work with</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'home'
}
</script>

<style lang="scss">
$pinkColor: rgba(232, 53, 86, 1);
$pinkColorHover: rgba(155, 36, 57, 1);
$cloudColor: rgba(97, 208, 212, 1);
$cloudColorHover: rgba(65, 139, 141, 1);
$stickyRiceColor: rgba(209, 201, 38, 1);
$stickyRiceColorHover: rgba(139, 134, 25, 1);

.pink-color {
  background-color: $pinkColor;
}

.cloud-color {
  background-color: $cloudColor;
}

.sticky-rice-color {
  background-color: $stickyRiceColor;
}
.home {
  .figure {
    width: 385px;
    height: 380px;
    border-radius: 50%;
    overflow: hidden;
    .figure-img {
      width: 100%;
      height: 100%;
      object-fit: cover;
    }
  }
}

.navigation-main {
  .nav-main-item {
    text-transform: uppercase;
    color: #ffffff;
    display: block;
    width: 130px;
    height: 130px;
    border-radius: 50%;
    box-sizing: border-box;
    text-align: center;
    line-height: 130px;
    transition: border 0.4s ease 0s, background-color 0.4s ease 0s;
    text-decoration: none;
    &.pink-color:hover {
      background-color: $pinkColorHover;
    }
    &.cloud-color:hover {
      background-color: $cloudColorHover;
    }
    &.sticky-rice-color:hover {
      background-color: $stickyRiceColorHover;
    }
  }
}

@media (max-width: 576px) {
  .home {
    .figure {
      width: 150px;
      height: 150px;
    }
    .nav-main-item {
      width: 100px;
      height: 100px;
      line-height: 100px;
    }
  }
}
</style>
