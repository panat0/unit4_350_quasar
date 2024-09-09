<template>
  <div class="htmlClass">
    <h1>{{ title }}</h1>
    <form>
      <input type="text" id="firstName" v-model="firstName" />
      <input type="text" id="secondName" v-model="secondName" />
      <input type="text" id="nickname" v-model="nickname" />
      <input type="text" id="studentcode" v-model="studentcode" />
      <button @click="submitForm()" class="submitForm">Submit</button>
  </form>
  </div>
</template>

<script>
export default {
  name: 'InputPage',
  data() {
    return {
      title: 'Input Page.',
      firstName: 'Peeraphat',
      secondName: 'Micranuch',
      nickname: 'Fook',
      studentcode: '6604101361',
    }
  },
  methods: {
    submitForm() {
      this.$emit('submit form')
    },
  }
}
</script>

