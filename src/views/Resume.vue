<template>
  <div class="container-fluid">
    <div class="row">
      <div class="col-sm-8">
        <ResumeRow />
        <ResumeRow />
      </div>
      <div class="col-sm-2">
        <div class="row">
          <div class="col-6 col-sm-12 resume-skills mb-4">
            <span class="label">
              <i class="fa fa-exclamation" aria-hidden="true"></i>
            </span>
            <span>Skills</span>
            <div class="hr"></div>
            <div class="font-13">
              <div class="text-uppercase">PHOTOSHOP FLASH
              </div>
              <p class="pt-2">Click to add a skill Click to add a skill Click to add a skill</p>
            </div>
          </div>
          <div class="col-6 col-sm-12 resume-language">
            <span class="label">
              <i class="fa fa-globe" aria-hidden="true"></i>
            </span>
            <span>Languages</span>
            <div class="hr"></div>
            <div class="font-13">
              <div class="text-uppercase">PHOTOSHOP FLASH
              </div>
              <p class="pt-2">Click to add a skill Click to add a skill Click to add a skill</p>
            </div>
          </div>
        </div>
      </div>
    </div>

  </div>
</template>

<script>
import ResumeRow from '@/components/Resume/ResumeRow.vue'

export default {
  name: 'resume',
  components: {
    ResumeRow
  }
}
</script>

<style lang="scss" scoped>
$cloudColor: rgba(97, 208, 212, 1);
$borderColor: rgba(139, 139, 139, 1);

.font-13 {
  font-size: 13px;
}
.resume-skills,
.resume-language {
  .label {
    width: 45px;
    height: 45px;
    display: block;
    background-color: $cloudColor;
    color: #ffffff;
    border-radius: 50%;
    text-align: center;
    line-height: 45px;
    margin-bottom: 15px;
  }
  .hr {
    border-top: 1px solid $borderColor;
    margin: 10px 0px;
  }
}
</style>
