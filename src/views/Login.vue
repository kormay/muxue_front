<template>
  <div id="login_form">
    <el-row :gutter="24" style="text-align: center">
      <el-col :xs="4" :sm="6" :md="8" :lg="8" :xl="8">&nbsp;</el-col>
      <el-col :xs="16" :sm="12" :md="8" :lg="8" :xl="8" id="login_div" style="padding-left: 50px; padding-right: 50px">
        <el-form :model="form" status-icon :rules="rules" ref="form" label-width="0" class="demo-form">
          <el-form-item label="" prop="account">
            <el-input type="text" v-model="form.account" autocomplete="off" placeholder="请输入用户名"></el-input>
          </el-form-item>
          <el-form-item label="" prop="pass">
            <el-input type="password" v-model="form.pass" autocomplete="off" placeholder="请输入密码"></el-input>
          </el-form-item>
          <el-form-item>
            <el-button type="success" @click="submitForm('form')" round>Yes, I like you</el-button>
          </el-form-item>
        </el-form>
      </el-col>
    </el-row>
  </div>
</template>

<style>
  body {
    background: url(../assets/backend.jpeg);
    background-size: 100% auto;
  }

  #login_div {
    padding-top: 50px;
    background:rgba(0,0,0,0.7);
    background-size: cover;
    border-radius: 10px;
  }

  #login_form {
    margin-top: 100px;
  }


</style>

<script>
  export default {
    data() {
      return {
        form: {
          account: '',
          pass: '',
        },
        rules: {
          account: [
            {required: true, message: '请输入用户名', trigger: 'blur'}
          ],
          pass: [
            {required: true, message: '请输入密码', trigger: 'blur'}
          ]
        }
      }
    },
    methods: {
      submitForm(formName) {
        this.$refs[formName].validate((valid) => {
          if (valid) {
            this.$router.push({name: "home"})
          } else {
            console.log('error submit!!')
            return false
          }
        })
      },
    }
  }
</script>
