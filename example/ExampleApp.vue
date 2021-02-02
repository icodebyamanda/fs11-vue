<template>
  <div class="container">
    <div>this is the App compoennt</div>
    <!-- 3. use it! -->
    <!-- <HelloWorld /> -->
    Enter here the max for the first counter:
    <input type="number" v-model="limitCounter1" />
    ​ just paint the number <ColorNumber :number="5" />
    ​
    <Counter :max="limitCounter1" />
    ​
    <Counter :max="20" />
    ​
    <Bank />
  </div>
</template>
​
<script>
// 1 import!
// import HelloWorld from "@/components/HelloWorld";
import Counter from "@/components/Counter";
import Bank from "@/components/Bank";
import ColorNumber from "@/components/ColorNumber";
​
export default {
  name: "App",
  data() {
    return {
      limitCounter1: 10,
    };
  },
  // 2 declare!
  components: {
    // HelloWorld,
    Counter,
    Bank,
    ColorNumber,
  },
};
</script>
​
<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
