<template>
  <span :class="{ 'text-danger': number <= 0, 'text-success': number > 0 }">{{
    number
  }}</span>
</template>
​
<script>
export default {
  props: ["number"]
};
</script>
​
<style></style>
