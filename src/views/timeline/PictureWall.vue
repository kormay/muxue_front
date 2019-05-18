<template>
  <div id="id_wall">
    <div class="wall-img">
      <el-row type="flex" class="row-bg move-up">
        <el-col :span="2"><img src="../../assets/kiss/kiss1.jpeg" alt=""></el-col>
        <el-col :span="2"><img src="../../assets/kiss/kiss2.jpeg" alt=""></el-col>
        <el-col :span="2"><img src="../../assets/kiss/kiss3.jpeg" alt=""></el-col>
        <el-col :span="2"><img src="../../assets/kiss/kiss4.jpeg" alt=""></el-col>
        <el-col :span="2"><img src="../../assets/kiss/kiss5.jpeg" alt=""></el-col>
        <el-col :span="2"><img src="../../assets/kiss/kiss6.jpeg" alt=""></el-col>
        <el-col :span="2"><img src="../../assets/kiss/kiss7.jpeg" alt=""></el-col>
        <el-col :span="2"><img src="../../assets/kiss/kiss8.jpeg" alt=""></el-col>
        <el-col :span="2"><img src="../../assets/kiss/kiss9.jpeg" alt=""></el-col>
        <el-col :span="2"><img src="../../assets/kiss/kiss10.jpeg" alt=""></el-col>
        <el-col :span="2"><img src="../../assets/kiss/kiss11.jpeg" alt=""></el-col>
        <el-col :span="2"><img src="../../assets/kiss/kiss12.jpeg" alt=""></el-col>
      </el-row>
      <el-row type="flex" class="row-bg move-up">
        <el-col :span="2"><img src="../../assets/kiss/kiss13.jpeg" alt=""></el-col>
        <el-col :span="2"><img src="../../assets/kiss/kiss14.jpeg" alt=""></el-col>
        <el-col :span="2"><img src="../../assets/kiss/kiss15.jpeg" alt=""></el-col>
        <el-col :span="2"><img src="../../assets/kiss/kiss16.jpeg" alt=""></el-col>
        <el-col :span="2"><img src="../../assets/kiss/kiss17.jpeg" alt=""></el-col>
        <el-col :span="2"><img src="../../assets/kiss/kiss18.jpeg" alt=""></el-col>
        <el-col :span="2"><img src="../../assets/kiss/kiss19.jpeg" alt=""></el-col>
        <el-col :span="2"><img src="../../assets/kiss/kiss20.jpeg" alt=""></el-col>
        <el-col :span="2"><img src="../../assets/kiss/kiss1.jpeg" alt=""></el-col>
        <el-col :span="2"><img src="../../assets/kiss/kiss2.jpeg" alt=""></el-col>
        <el-col :span="2"><img src="../../assets/kiss/kiss3.jpeg" alt=""></el-col>
        <el-col :span="2"><img src="../../assets/kiss/kiss4.jpeg" alt=""></el-col>
      </el-row>
      <el-row type="flex" class="row-bg move-up">
        <el-col :span="2"><img src="../../assets/kiss/kiss5.jpeg" alt=""></el-col>
        <el-col :span="2"><img src="../../assets/kiss/kiss6.jpeg" alt=""></el-col>
        <el-col :span="2"><img src="../../assets/kiss/kiss7.jpeg" alt=""></el-col>
        <el-col :span="2"><img src="../../assets/kiss/kiss8.jpeg" alt=""></el-col>
        <el-col :span="2"><img src="../../assets/kiss/kiss9.jpeg" alt=""></el-col>
        <el-col :span="2"><img src="../../assets/kiss/kiss1.jpeg" alt=""></el-col>
        <el-col :span="2"><img src="../../assets/kiss/kiss2.jpeg" alt=""></el-col>
        <el-col :span="2"><img src="../../assets/kiss/kiss3.jpeg" alt=""></el-col>
        <el-col :span="2"><img src="../../assets/kiss/kiss4.jpeg" alt=""></el-col>
        <el-col :span="2"><img src="../../assets/kiss/kiss5.jpeg" alt=""></el-col>
        <el-col :span="2"><img src="../../assets/kiss/kiss6.jpeg" alt=""></el-col>
        <el-col :span="2"><img src="../../assets/kiss/kiss7.jpeg" alt=""></el-col>
      </el-row>
    </div>
    <div class="wall-content">
      <el-row>
        <el-col :span="24" class="love-word">Xue, I have fallen in love with you for</el-col>
        <el-col :span="24">
          <span class="last-time"> {{days}} </span>
          <span class="last-unit">days</span>
          <span class="last-time"> {{hours}} </span>
          <span class="last-unit">hours</span>
          <span class="last-time"> {{minutes}} </span>
          <span class="last-unit">minutes</span>
          <span class="last-time"> {{seconds}} </span>
          <span class="last-unit">seconds</span>
        </el-col>
      </el-row>
    </div>
  </div>
</template>

<style>
  @font-face {
    font-family: digit;
    src: url("../../assets/digital-7_mono.ttf") format("truetype");
  }
  .wall-img {
    background-color: black;
  }

  .wall-img img {
    width: 100%;
    height: 100%;
    opacity: 0.4;
  }

  .wall-content {
    margin-top: -15%;
    margin-bottom: 15%;
    color: #f7f7f7;
    -ms-text-align-last: right;
    text-align: center;
  }

  .love-word {
    font-family: sans-serif;
    font-size: 3.2em;
  }
  .last-time {
    font-family: "digit";
    font-size: 4em;
  }
  .last-unit {
    font-size: 2em;

  }
</style>

<script>
  export default {
    data () {
      return {
        days: '231',
        hours: '13',
        minutes: '29',
        seconds: '21',
      }
    },
  }
</script>
