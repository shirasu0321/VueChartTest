<template>
  <div id="Home">
    <Dashboad/>
    <span class="icon is-large">
      <span class="fa-stack">
        <a class="is-large far fa-address-card" @click="openModal"></a>
      </span>
    </span>
    <SearchModal  @close="closeModal" v-if="modal">
    </SearchModal>
  </div>
</template>

<script>
import Dashboad from "../components/Dashboad";
import SearchModal from "./SearchPanel";

export default {
  components: {
    Dashboad,
    SearchModal
  },
  data() {
    return {
      modal: false,
      message: ""
    };
  },
  methods: {
    openModal() {
      this.modal = true;
    },
    closeModal() {
      this.modal = false;
    }
  }
};
</script>

<style scoped>
#Home {
  height: 100%;
  width: 100%;
  background-color: #b0c4de;
}
</style>
