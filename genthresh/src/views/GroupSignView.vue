<template>
    <TitleCard title="Group Sign" />
    <div class="flex flex-wrap flex-row justify-center gap-1 pb-5 mx-10">
      <mainButton title="✨ New Group" />
      <mainButton title="👨‍👩‍👧‍👦 Existing Group" />
    </div>

  </template>
  
  <script>
  import { defineComponent } from "vue";
  
  // Components
  import TitleCard from "@/components/TitleCard.vue";
  import mainButton from "@/components/mainButton.vue";
  
  export default defineComponent({
    name: "GroupSignView",
  
    components: {
      TitleCard,
      mainButton,
    },
  });
  </script>