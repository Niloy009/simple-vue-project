<template>
  <div id="programmers">
    <h1>Programmers</h1>
    <ul>
      <li v-for="programmer in programmers"
          v-on:click="programmer.show = !programmer.show">
        <h2>{{ programmer.name }}</h2>
        <h3 v-show="programmer.show">Skills: {{ programmer.skill }}</h3>
      </li>
    </ul>
  </div>
</template>

<script>

export default {

  data() {
    return {
      programmers: [
        {name: 'Niloy Saha Roy', skill: 'VueJS, Laravel', show: false},
        {name: 'Jabid Hasan', skill: 'ReactJS, Laravel', show: false},
        {name: 'MD Rayhan', skill: 'VueJS, NodeJS', show: false},
        {name: 'Shoaib Sharif', skill: 'ReactJS, NodeJS', show: false},
      ]
    }
  }
}
</script>

<style scoped>
h1{
  text-align: center;
}

#programmers {
  width: 100%;
  max-width: 1200px;
  margin: 40px auto;
  padding: 0 20px;
  box-sizing: border-box;
}

ul {
  display: flex;
  flex-wrap: wrap;
  list-style-type: none;
  padding: 0;
}

li {
  flex-grow: 1;
  flex-basis: 300px;
  text-align: center;
  padding: 30px;
  border: 1px solid #222;
  margin: 10px;
}

</style>
