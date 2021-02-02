<template>
  <div>
    <div>The message is {{ message }}</div>
    <input type="text" v-model="message" />
  </div>
</template>
​
<script>
export default {
  data() {
    return {
      message: ""
    };
  }
};
</script>
​
<style></style>
