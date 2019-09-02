<template>
  <div class="hello">
    <p>{{number}}</p>
    <button v-on:click="clickPlus">{{ click1 }}</button>
    <button v-on:click="clickMun">{{ click2 }}</button>
  </div>
</template>

<script>
export default {
  name: "Counter",
  props: {
    msg: String
  },
  data() {
    return {
      number: 0,
      click1: "+",
      click2: "-"
    };
  },
  methods: {
    clickPlus: function() {
      this.number++;
    },
    clickMun: function() {
      this.number--;
    }
  }
};
</script>