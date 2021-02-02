<template>
  <div class="card card-body mb-4">
    <div>
      Count up to {{ max }}: ​
      <ColorNumber :number="count" />
    </div>
    <div>
      <button @click="increase" class="btn btn-dark">+1</button>
      <button @click="decrease" class="btn btn-dark">-1</button>
    </div>
  </div>
</template>
​
<script>
import ColorNumber from "@/components/ColorNumber";
​
export default {
  components: {
    ColorNumber,
  },
  props: ["max"],
  data() {
    return {
      count: 0,
    };
  },
  methods: {
    increase() {
      if (this.count < this.max) this.count++;
    },
    decrease() {
      if (this.count > 0) this.count--;
    },
  },
};
</script>
​
<style></style>
