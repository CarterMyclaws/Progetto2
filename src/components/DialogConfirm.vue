<template>
  <div>
    <md-dialog-confirm
      :md-active.sync="active"
      md-title="Are you sure you want to Logout?"
      md-confirm-text="CONFIRM"
      md-cancel-text="CANCEL"
      @md-cancel="onCancel"
      @md-confirm="onConfirm"
    />
    <p v-if="username">Hi {{username}}!</p>
    <md-button v-if="username" class="md-primary md-raised" @click="active = true">Logout</md-button>
  </div>
</template>

<script>
import DataService from "../dataservice";
export default {
  name: "DialogConfirm",
  data: () => ({
    active: false,
    value: null,
    username: null
  }),
  methods: {
    onConfirm() {
      DataService.logout();
      this.$router.push({ path: "/Login" });
      /* this.value = "Conferma"; */
    },
    onCancel() {
      this.value = "Cancella";
    }
  },
  created: function() {
    this.username = DataService.whoIsAuthenticated();
  }
};
</script>