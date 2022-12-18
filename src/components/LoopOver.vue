<template>
  <div>
    <h1>Looping through arrays</h1>
    <ul>
      <li v-for="n in 5" :key="n">
        {{ n }}
      </li>
    </ul>
    <ul>
      <li v-for="(item, n) in interests" :key="n">
        {{ item }}
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  data(){
    return {
      interests:['TV','Movies','Music','Books','Sports','Food','Travel','Fashion','Gaming','Art','Photography','Science','Technology','Nature','Animals','Cars','Fitness','Health','History','Politics','Religion','Spirituality','Family','Friends','Work','Money','Education','Philosophy','Psychology','Relaxation','Humor','Other'],
    }
  },
}
</script>

<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
