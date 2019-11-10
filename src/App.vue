<template>
  <div id="app">
    <textarea v-model="commands"></textarea>
    <button v-on:click="commandList=commands.split('\n')">Plot</button>
    <Output :commandList="commandList" />
  </div>
</template>

<script>
import Output from "./components/Output";

export default {
  name: "app",
  components: {
    Output
  },
  methods: {
    reader() {
      this.test = this.circle.cx.split("\n");
    }
  },
  data() {
    return {
      commands: `p   200  ,10                250,  190 160 , 210  \n \nc          20  100  20\nr 100   50            25  25  \nR  50 150.00  50 25  `,
      commandList: []
    };
  }
};
</script>

<style>
body {
  background: #ffeaa7;
  padding-top: 200px;
  display: flex;
  justify-content: center;
}

textarea {
  width: 250px;
  height: 100px;
}

button {
  display: block;
  margin: 10px auto 20px;
  padding: 15px 50px;
  font-size: 24px;
  cursor: pointer;
  text-align: center;
  text-decoration: none;
  outline: none;
  color: #fff;
  background-color: #4caf50;
  border: none;
  border-radius: 15px;
  box-shadow: 0 9px #999;
}

button:hover {
  background-color: #3e8e41;
}

button:active {
  background-color: #3e8e41;
  box-shadow: 0 5px #666;
  transform: translateY(4px);
}
</style>
