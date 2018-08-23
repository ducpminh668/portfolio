<template>
  <footer>
    <div class="footer-contact">
      <div class="container-fluid">
        <div class="row">
          <div class="col-sm-3">
            <div class="footer-contact-item d-flex flex-row align-items-center">
              <a href="" class="d-block">
                <i class="fa fa-phone" aria-hidden="true"></i>
              </a>
              <div>
                <div>Call</div>
                <div>T:123-456-7890</div>
                <div>F:123-456-7890</div>
              </div>
            </div>
          </div>
          <div class="col-sm-3">
            <div class="footer-contact-item d-flex flex-row align-items-center">
              <a href="" class="d-block">
                <i class="fa fa-phone" aria-hidden="true"></i>
              </a>
              <div>
                <div>Call</div>
                <div>T:123-456-7890</div>
                <div>F:123-456-7890</div>
              </div>
            </div>
          </div>
          <div class="col-sm-3">
            <div class="footer-contact-item d-flex flex-row align-items-center">
              <a href="" class="d-block">
                <i class="fa fa-phone" aria-hidden="true"></i>
              </a>
              <div>
                <div>Call</div>
                <div>T:123-456-7890</div>
                <div>F:123-456-7890</div>
              </div>
            </div>
          </div>
          <div class="col-sm-3">
            <div class="footer-contact-item d-flex flex-row align-items-center">
              <a href="" class="d-block">
                <i class="fa fa-phone" aria-hidden="true"></i>
              </a>
              <div>
                <div>Call</div>
                <div>T:123-456-7890</div>
                <div>F:123-456-7890</div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="footer-bottom d-none d-sm-block"></div>
  </footer>
</template>

<script>
export default {}
</script>

<style lang="scss">
$pinkColor: rgba(232, 53, 86, 1);
$height: 137px;

footer {
  color: #ffffff;
  background-color: $pinkColor;
  margin-top: 50px;
  .footer-contact {
    margin-left: calc((100% - 980px) / 2);
    width: 980px;
    .footer-contact-item {
      height: $height;
      a {
        width: 45px;
        height: 45px;
        background-color: red;
        text-align: center;
        line-height: 45px;
        border-radius: 50%;
        margin-right: 20px;
        background-color: rgba(97, 208, 212, 1);
        .fa {
          font-size: 25px;
          color: $pinkColor;
          line-height: 45px;
        }
      }
    }
  }
}
.footer-bottom {
  background-color: #eae5e5;
  height: 50px;
}

@media (max-width: 576px) {
  footer {
    margin: 10px 0;
    .footer-contact {
      margin-left: 0;
      width: 100%;
      .footer-contact-item {
        height: 100px;
      }
    }
  }
}
</style>
