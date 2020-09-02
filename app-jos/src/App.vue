<template>
  <div>
    <!-- <p>hello belajar vuejs</p>
    <NewComponent :name="user"/> -->
    <span v-bind:title="pesan">
    Arahkan mouse Anda kesini dan tunggu dalam beberapa detik
    untuk melihat judul pesan yang dinamis
  </span>
  </div>
</template>

<script>
// import NewComponent from './components/NewComponent.vue'
export default {
  data: ()=> {
    return {
      // user: "walid"
      pesan: 'Anda memuat halaman ini pada jam ' + new Date().toLocaleString()
    }
  },
  // name: 'App',
  // components: {
  //   NewComponent,
  //  }
}
</script>

<style>

</style>
