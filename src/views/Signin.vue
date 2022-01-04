<template>
  <h1>Signin</h1>
  <div class="row">
    <div class="col-md-6 mx-auto mt-3">
      <form @submit.prevent="signin">
        <div class="form-group mb-2">
          <label for="Email">Email</label>
          <input type="Email" v-model="user.email" class="form-control" name="Email" id="Email">
        </div>
        <div class="form-group mb-2">
          <label for="Password">Password</label>
          <input type="Password" v-model="user.password" class="form-control" name="Password" id="Password">
        </div>
        <button class="btn btn-primary w-100">Singn in</button>
      </form>
    </div>
  </div>
</template>

<script>
import axios from 'axios';
export default {
  data(){
    return{
      user:{
        email:'',
        password:''
      }
    }
  },
  methods:{
    async signin(){
      const response= await axios.post('http://localhost:8000/api/auth/login',this.user)
      console.log(response.data)
    }
  }
}
</script>
