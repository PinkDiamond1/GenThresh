<template>
    <contenteditable tag="div" :contenteditable="isEditable" v-model="message" :noNL="true" :noHTML="true" @returned="enterPressed" />
</template>
   
  <script>
  import contenteditable from 'vue-contenteditable'; // Not needed it registered globally
  export default {
    components : {
      contenteditable
    }, // Not needed it registered globally
    data() {
      return {
        isEditable: true,
        message: ""
      }
    },
    methods : {
      enterPressed(){
        alert('Enter Pressed');
      }
    }
  }
  </script>