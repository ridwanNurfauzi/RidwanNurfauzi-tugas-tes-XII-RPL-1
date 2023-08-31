<template>
  <div class="min-h-screen">
    <div class="flex flex-col min-h-screen">
      <div class="sticky top-0 left-0">
        <Navbar :id-menu="idMenu" :key="idMenu"></Navbar>
      </div>
      <div class="flex-1 flex flex-col bg-gray-50">
        <RouterView @id-menu="setMenu($event)"></RouterView>
      </div>
    </div>
  </div>
</template>

<script>
import { ref } from "vue";
import Navbar from './components/Navbar.vue';

export default {
  components: {
    Navbar
  },
  setup() {
    const idMenu = ref(0);

    function setMenu(id) {
      idMenu.value = id;
    }
    return {
      idMenu,
      setMenu
    }
  }
}
</script>
