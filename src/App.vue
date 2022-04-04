<template>
  <div class="container; background" style="font-family: serif">
    <form @submit.prevent="submitForm">
      <div>회원가입 페이지</div>
      <div>
        <label for="email">email</label>
        <input type="text" id="email" v-model="email"/>
      </div>
      <div>
        <label for="name">이름</label>
        <input type="text" id="name" v-model="name"/>
      </div>
      <div>
        <label for="password">비밀번호</label>
        <input type="password" id="password" v-model="password"/>
      </div>
      <div>
        <label for="passwordConfirm">비밀번호확인</label>
        <input type="password" id="passwordConfirm" v-model="passwordConfirm"/>
      </div>
      <button style="padding: 2px 10px" type="submit">확인</button>
    </form>
  </div>

</template>

<script>



export default {
  name: 'SignupForm',
  data() {
    return{
      email: '',
      name: '',
      password: '',
      passwordConfirm: '',
    };
  },
  methods: {
    submitForm() {
      console.log('dd')
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
}

.background {
  height: 100vh;
  overflow: hidden;
  margin: 0;
  background-color: beige;
  background-size: cover;
  background-repeat: no-repeat;
  background-position: center;
}

.css {
  width: 1600px;
  height: 50px;
  background: rgb(219, 219, 245);
  text-align: center;
  line-height: 30px;
  box-sizing: border-box;
}


</style>
