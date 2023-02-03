<script>
import AppHeader from './components/AppHeader.vue'
import AppMain from './components/AppMain.vue'
import AppFooter from './components/AppFooter.vue'

export default {
  name: 'Marketing Consultant',
  components: { AppHeader, AppMain, AppFooter },
  data() {
    return {
      name: '',
      email: '',
      phone: ''
    }
  },
  methods: {
    fillData(name) {
      this.name = name
    }
  }
}
</script>

<template>

  <AppHeader></AppHeader>
  <AppMain @name-submit="fillData"></AppMain>
  <AppFooter></AppFooter>
  <div class="support">
    <i class="fa-solid fa-comments"></i>
  </div>
</template>

<style lang="scss" scoped>
@use './assets/scss/partials/variables' as *;

.support {
  position: sticky;
  bottom: 0;
  left: 10000px;
  height: 70px;
  width: 1200px;
}

.fa-comments {
  color: $white;
  background-color: $ochre;
  padding: 1rem;
  margin-left: 2rem;
  border-radius: 5rem;

  cursor: pointer;

}
</style>
