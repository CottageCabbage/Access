<template id="app">
  <SidebarComponent />
  <main>
    <router-view/>
    asd
    <Menubar :model="items" class="menubar"/>
  </main>
</template>

<script>
import SidebarComponent from '@/components/SidebarComponent.vue'
import Menubar from 'primevue/menubar';

export default {
  components: {
    SidebarComponent,
    Menubar
  },
  data () {
    return {
      items: [
        {
          label: "User",
          items: [{label: "Thing"}, {label: "Another thing"}]
        }
      ]
    }
  }
}
</script>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

html, body, #app {
  height: 100%;
}

#app {
  display: flex;
}
main {
  display: flex;
  flex-direction: column;
  height: 100%;
}

.menubar {
  margin-top: auto;
}
</style>
