<template>
  <div id="menu-title">
    <el-row class="kiss-title">
      <el-col :span="1"><img class="kiss-icon" src="../assets/kiss/kiss1.jpeg" alt=""></el-col>
      <el-col :span="1"><img class="kiss-icon" src="../assets/kiss/kiss2.jpeg" alt=""></el-col>
      <el-col :span="1"><img class="kiss-icon" src="../assets/kiss/kiss3.jpeg" alt=""></el-col>
      <el-col :span="1"><img class="kiss-icon" src="../assets/kiss/kiss4.jpeg" alt=""></el-col>
      <el-col :span="1"><img class="kiss-icon" src="../assets/kiss/kiss5.jpeg" alt=""></el-col>
      <el-col :span="1"><img class="kiss-icon" src="../assets/kiss/kiss6.jpeg" alt=""></el-col>
      <el-col :span="1"><img class="kiss-icon" src="../assets/kiss/kiss7.jpeg" alt=""></el-col>
      <el-col :span="1"><img class="kiss-icon" src="../assets/kiss/kiss8.jpeg" alt=""></el-col>
      <el-col :span="1"><img class="kiss-icon" src="../assets/kiss/kiss9.jpeg" alt=""></el-col>
      <el-col :span="1"><img class="kiss-icon" src="../assets/kiss/kiss10.jpeg" alt=""></el-col>
      <el-col :span="1"><img class="kiss-icon" src="../assets/kiss/kiss11.jpeg" alt=""></el-col>
      <el-col :span="1"><img class="kiss-icon" src="../assets/kiss/kiss12.jpeg" alt=""></el-col>
      <el-col :span="1"><img class="kiss-icon" src="../assets/kiss/kiss13.jpeg" alt=""></el-col>
      <el-col :span="1"><img class="kiss-icon" src="../assets/kiss/kiss14.jpeg" alt=""></el-col>
      <el-col :span="1"><img class="kiss-icon" src="../assets/kiss/kiss15.jpeg" alt=""></el-col>
      <el-col :span="1"><img class="kiss-icon" src="../assets/kiss/kiss16.jpeg" alt=""></el-col>
      <el-col :span="1"><img class="kiss-icon" src="../assets/kiss/kiss17.jpeg" alt=""></el-col>
      <el-col :span="1"><img class="kiss-icon" src="../assets/kiss/kiss18.jpeg" alt=""></el-col>
      <el-col :span="1"><img class="kiss-icon" src="../assets/kiss/kiss19.jpeg" alt=""></el-col>
      <el-col :span="1"><img class="kiss-icon" src="../assets/kiss/kiss20.jpeg" alt=""></el-col>
      <el-col :span="1"><img class="kiss-icon" src="../assets/kiss/kiss21.jpeg" alt=""></el-col>
      <el-col :span="1"><img class="kiss-icon" src="../assets/kiss/kiss22.jpeg" alt=""></el-col>
      <el-col :span="1"><img class="kiss-icon" src="../assets/kiss/kiss23.jpeg" alt=""></el-col>
      <el-col :span="1"><img class="kiss-icon" src="../assets/kiss/kiss24.jpeg" alt=""></el-col>
      <!--<el-col :span="2"><div :span="2" class="kiss-icon"><img src="../assets/kiss/kiss15.jpeg" alt=""></div></el-col>-->
      <!--<el-col :span="2"><div :span="2" class="kiss-icon"><img src="../assets/kiss/kiss16.jpeg" alt=""></div></el-col>-->
      <!--<el-col :span="2"><div :span="2" class="kiss-icon"><img src="../assets/kiss/kiss17.jpeg" alt=""></div></el-col>-->
      <!--<el-col :span="2"><div :span="2" class="kiss-icon"><img src="../assets/kiss/kiss18.jpeg" alt=""></div></el-col>-->
    </el-row>
  </div>
</template>

<style>
  .kiss-title {
    width: 100%;
    background: lightpink;
  }
  .kiss-icon {
    width: 100%;
    border-radius: 50%;
  }
</style>

<script>
  export default {
    name: "menu-title",
    data() {
      return {
        activeIndex: '1',
        activeIndex2: '1'
      };
    },
    methods: {
      handleSelect(key, keyPath) {
        console.log(key, keyPath);
      }
    }
  }
</script>
