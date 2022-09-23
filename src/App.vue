<template>
  <h1>send data from parent to child</h1>
  <!-- <parent-tochild
    :FirstName="FirstName"
    :LastName="LastName"
    :RollNo="RollNo"
  /> -->
  <!-- <parent-to-child-1 :things="things" /> -->
  <!-- <parent-to-child-2 greeting="Hello Good Morning" /> -->
  <child-to-parent @add="add" />
  <h1>{{ value }}</h1>
  <child-to-parent-1 @idData="idData" />
  <h1>{{ iddata }}</h1>
  <child-to-parent-2 @ageData="ageData" />
  <h1>{{ agedata }}</h1>
  <child-to-parent-3 @addData="addData" />
  <h1>{{ adddata }}</h1>
  <child-to-parent-4 @subData="subData" />
  <h1>{{ subdata }}</h1>
  <conditional-rendering />
  <con-red />
</template>

<script>
import ChildToParent2 from "./components/ChildToParent 2.vue";
import ChildToParent3 from "./components/ChildToParent 3.vue";
import ChildToParent4 from "./components/ChildToParent 4.vue";
import ChildToParent from "./components/ChildToParent.vue";
import ChildToParent1 from "./components/ChildToParent1.vue";
import ConditionalRendering from "./components/ConditionalRendering.vue";
import ConRed from "./components/ConRed.vue";
// import ParentToChild2 from "./components/ParentToChild2.vue";
// import ParentTochild from "./components/ParentTochild.vue";
// import ParentToChild1 from "./components/ParentToChild1.vue";
export default {
  name: "App",
  components: {
    ChildToParent,
    ChildToParent1,
    ChildToParent2,
    ChildToParent3,
    ChildToParent4,
    ConditionalRendering,
    ConRed,
    // ParentToChild2,
    // ParentTochild,
    // ParentToChild1,
  },
  data() {
    return {
      FirstName: "Nuthana",
      LastName: "T G",
      RollNo: 22,
      things: ["pen", "book", "pencile", "playwood", "paper"],
      value: "",
      iddata: "",
      agedata: "",
      adddata: "",
      subdata: "",
    };
  },
  methods: {
    add(child) {
      console.log("chocholate function executed", child);
      this.value = child;
    },
    idData(child) {
      this.iddata = child;
    },
    ageData(child) {
      this.agedata = child;
    },
    addData(child) {
      this.adddata = child;
    },
    subData(child) {
      this.subdata = child;
    },
  },
};
</script>

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
