<template>
  <div class="d-flex flex-row resume-row">
    <div class="resume-row-label">
      <span>
        Professional Info
      </span>
    </div>
    <div class="resume-row-description">I'm a paragraph. Click here to add your own text and edit me. It’s easy. Just click “Edit Text” or double click me and you can start adding your own content and make changes to the font. Feel free to drag and drop me anywhere you like on your page. I’m a great place for you to write more. Tell a story about yourself.</div>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
$pinkColor: rgba(232, 53, 86, 1);
$borderTopColor: rgba(139, 139, 139, 1);

.resume-row {
  border-top: 1px solid $borderTopColor;
  padding: 30px 20px 50px 10px;
  .resume-row-label {
    width: 25%;
    span {
      width: 120px;
      height: 120px;
      display: block;
      border-radius: 50%;
      background-color: $pinkColor;
      text-align: center;
      padding: 20px;
      display: flex;
      align-items: center;
      color: #ffffff;
    }
  }
  .resume-row-description {
    width: 80%;
    text-align: justify;
    padding-top: 30px;
  }
}

@media (max-width: 576px) {
  .resume-row {
    .resume-row-label {
      span {
        width: 76px;
        height: 76px;
        font-size: 11px;
        padding: 0;
        overflow: hidden;
      }
    }
    .resume-row-description {
      padding-left: 20px;
      padding-top: 10px;
    }
  }
}
</style>
