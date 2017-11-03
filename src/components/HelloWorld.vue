<template>
  <div>
    <h1>OI! :)</h1>
    <h2>Pronto para detonar!</h2>
  </div>
</template>

<script>
export default {
  data: {
    form: {
      email: '',
      name: '',
      food: null,
      checked: false,
      secret: 'S3CR3T'
    },
    foods: [
      'Carrots', 'Beans', 'Tomatoes', 'Corn'
    ]
  },
  methods: {
    onSubmit (evt) {
      evt.preventDefault()
      alert(JSON.stringify(this.form))
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
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
