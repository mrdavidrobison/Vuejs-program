/* eslint-disable */

<template>
  <div class="test">
    <h1>{{fruit[1]}}</h1>
    <h1>{{veggies[1]}}</h1>
    <p v-text="product.bowls[1]"></p>
    <p v-html="product.bowls[0]"></p>
    <p v-if="!showVeggie">{{veggies[1]}}</p>
    <ul>
      <li v-for="chain in chains">{{chain.id}}</li>
    </ul>
    <input type='text' v-model='veggies[1]'>
    <button v-on:click="sayHello()">Say Hello</button>
    <h1>{{message}}</h1>

  </div>
</template>

<script>
export default {
  name: 'test',
  props: {
    message: {
      type: String,
      default: 'hey fellas'
    }
  },
  data () {
    return {
      fruit: ['apple', 'banana', 'cherry'],
      veggies: ['broccoli', 'potato', 'asparagus'],
      product: {
        bowls: ['<h1>ceramic</h1>', '<h3>glass</h3>']
      },
      chains: [
        {id: '38299'},
        {id: '8372487'},
        {id: '1238948'}
      ],

      showName: false

    }
  },
  methods: {
    sayHello: function () {
      alert('what up?')
    }
  }
}

</script>

<style scoped>

</style>
