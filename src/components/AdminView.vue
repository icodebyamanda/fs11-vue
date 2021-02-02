<template>
  <div>
    Title
    <input v-model="title" />
    Description
    <input v-model="description" />
    Image
    <input :href="url" />
    <!-- to display: https://vuejs.org/v2/guide/components-custom-events.html -->
    <button @click="handleSubmit">SUBMIT</button>
  </div>
</template>

<script>
export default {
  name: "AdminView",
  data() {
    return {
      title: "",
      image: "",
      description: ""
    };
  },
  methods: {
    handleSubmit() {
      this.$emit("createProject", {
        title: this.title,
        image: this.image,
        description: this.description
      });
    }
  }
};
</script>

<style></style>
