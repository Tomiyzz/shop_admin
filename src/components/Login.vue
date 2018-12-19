<template>
  <div class="login">

    <el-form ref="form" :model="form" label-width="80px">
      <img src="../assets/563253387983844822.jpg" alt="">
      <el-form-item label="用户名">
        <el-input v-model="form.username"></el-input>
      </el-form-item>
      <el-form-item label="密码">
        <el-input v-model="form.password"></el-input>
      </el-form-item>
      <el-form-item>
        <el-button type="primary" @click="onSubmit">立即创建</el-button>
        <el-button>取消</el-button>
      </el-form-item>
    </el-form>
  </div>
</template>

<script>
export default {
  data () {
    return {
      form: {
        username: '',
        password: ''
      }
    }
  },
  methods: {
    onSubmit () {
      console.log('submit!')
    }
  }
}
</script>

<style lang="less">
  .login {
    height: 100%;
    width: 100%;
    background-color: #2d434c;
    overflow: hidden;
    .el-form {
      width: 400px;
      background-color: #fff;
      margin: 200px auto;
      padding: 75px 40px 15px;
      position: relative;
      img {
        width: 120px;
        height: 120px;
        position: absolute;
        left: 50%;
        transform: translate(-50%);
        top: -70px;
        border-radius: 50%;
        border: 10px solid #fff;
      }
    }
  }
</style>
