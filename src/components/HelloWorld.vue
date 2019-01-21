<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    {{ num }}
    <div class="control">
      <button class="button is-primary" v-on:click=metode1(5)>Submit</button>
    </div>
  </div>
</template>

<script>
export default {
    name: 'HelloWorld',
    props: {
      msg: String
    },
    methods: {
      metode1(p1){
          var num1 = 1;

          this.num = this.num + p1 + num1;
      }
    },
    data: function() {
        return {
            num: 0
        }
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
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
