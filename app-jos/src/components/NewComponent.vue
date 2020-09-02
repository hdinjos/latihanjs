<template>
  <div>
    <h1>Kami belajar vuejs dengan {{fruits}}?</h1>
    <ol>
      <li v-for="fruit in fruits" :key="fruit">
        <span v-if="fruit === 'mangga'">{{fruit}}</span>
        <span v-else>oke</span>
      </li>
    </ol>
    <p :title="learn">membuat web app dengan vuejs</p>
    <button v-on:click="warning(2,5)">Alert</button>
    <p>ini nama saya {{name}}</p>
  </div>
</template>

<script>
export default {
  data: ()=> {
    return {
      user: "hendi",
      fruits: ["mangga", "pepaya", "salak"],
      learn: "belajar js"
    }
  },
  methods: {
    warning: function(a,b) {
      alert(a+b);
    }
  },
  props: ['name']
}
</script>

<style scoped>
  div{
    background-color: red;
    color: white;
  }
</style>