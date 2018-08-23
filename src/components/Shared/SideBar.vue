<template>
  <div id="parentx">
    <vs-button @click="active=!active" class="openMenuButton d-block d-sm-none">
      <i class="fa fa-bars" aria-hidden="true"></i>
    </vs-button>
    <vs-sidebar :vs-active.sync="active">
      <vs-sidebar-item @click="actives=1" :vs-active="actives==1" vs-icon="question_answer">
        Dashboard
      </vs-sidebar-item>
      <vs-sidebar-item @click="actives=2" :vs-active="actives==2" vs-icon="gavel">
        History
      </vs-sidebar-item>
      <vs-sidebar-item @click="actives=3" :vs-active="actives==3" vs-icon="verified_user">
        Settings
      </vs-sidebar-item>
      <vs-sidebar-item @click="actives=4" :vs-active="actives==4" vs-icon="account_box">
        Profile
      </vs-sidebar-item>
      <vs-sidebar-item @click="actives=5" :vs-active="actives==5" vs-icon="card_giftcard">
        card
      </vs-sidebar-item>
    </vs-sidebar>
  </div>
</template>

<script>
export default {
  data: () => ({
    active: false,
    actives: 2
  })
}
</script>

<style scoped>
.openMenuButton {
  position: fixed;
  top: 20px;
  right: 20px;
  padding: 5px 11px;
  z-index: 9999;
}
.vs-button-primary.vs-button-filled {
  background-color: #9b9fa5;
}
</style>
