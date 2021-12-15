<template>
    <form action="#" @submit.prevent="handleLogin">
        
        <div class="row mb-3">
            <label for="email" class="col-md-4 col-form-label text-md-right">E-Mail Address</label>

            <div class="col-md-6">
                <input v-model="formData.email" id="email" type="email" class="form-control" name="email" required autocomplete="email" autofocus>
            </div>
        </div>

        <div class="row mb-3">
            <label for="password" class="col-md-4 col-form-label text-md-right">Password</label>

            <div class="col-md-6">
                <input v-model="formData.password" id="password" type="password" class="form-control" name="password" required autocomplete="current-password">
            </div>
        </div>

        <div class="row mb-3">
            <div class="col-md-6 offset-md-4">
                <div class="form-check">
                    <input class="form-check-input" type="checkbox" name="remember" id="remember" >

                    <label class="form-check-label" for="remember">
                      Remember Me
                    </label>
                </div>
            </div>
        </div>

        <div class="row mb-0">
            <div class="col-md-8 offset-md-4">
                <button type="submit" class="btn btn-primary">
                    Login
                </button>

                
                <a class="btn btn-link" href="#">
                    Forgot Your Password?
                </a>
                
            </div>
        </div>
    </form>
</template>

<script>
    export default {
        data() {
            return {
                secrets: [],
                formData: {
                    'email' : '',
                    'password' : ''
                }
            }
        },
        methods: {
            handleLogin(){
                axios.get('/sanctum/csrf-cookie').then(response => {
                    // Login...
                    //console.log(response);
                    axios.post('/login', this.formData).then(response=>{
                        console.log(response);
                    });
                });
            }
        },
        mounted() {
            console.log('Component mounted.')
        }
    }
</script>
