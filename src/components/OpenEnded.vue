<template>
  <div class="kaka">
      <h1>Open-Ended</h1>
      <form  @submit.prevent="question">
         <p>The answer to the question is: {{ answer }}</p>
         <textarea v-model="answer" placeholder="add multiple lines"></textarea>
         <button type="submit">Submit</button>
      </form>
  </div>
</template>

<script>
export default {
  name: 'OpenEnded',

  data() {
    return {
      answer: '',
    };
  },

  methods: {
    question() {
      console.log(this.answer);
    },
  },
};
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
