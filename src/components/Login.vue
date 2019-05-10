<template>
  <div id="login_form">
    <el-row :gutter="24">
      <el-col :span="8" :offset="8">
        <el-form :model="form" status-icon :rules="rules" ref="form" label-width="100px" class="demo-form">
          <el-form-item label="用户名" prop="account">
            <el-input type="text" v-model="form.account" autocomplete="off"></el-input>
          </el-form-item>
          <el-form-item label="密码" prop="pass">
            <el-input type="password" v-model="form.pass" autocomplete="off"></el-input>
          </el-form-item>
          <el-form-item>
            <el-button type="primary" @click="submitForm('form')">提交</el-button>
          </el-form-item>
        </el-form>
      </el-col>
    </el-row>
  </div>
</template>

<script>
  export default {
    data () {
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
      submitForm (formName) {
        this.$refs[formName].validate((valid) => {
          if (valid) {
            alert('submit!')
          } else {
            console.log('error submit!!')
            return false
          }
        })
      },
    }
  }
</script>
