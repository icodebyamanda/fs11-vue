<template>
  <div>
    Bank
    <div>
      Income:
      <ColorNumber :number="income" />
    </div>
    <div>
      Outcome:
      <ColorNumber :number="outcome" />
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
  data() {
    return {
      income: 100,
      outcome: -50,
    };
  },
};
</script>
​
<style></style>
