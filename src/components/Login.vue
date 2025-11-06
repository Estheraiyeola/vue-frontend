<script setup>
</script>
<template>
  

  <main class="login-layout">
    <div class="left">
        <div class="logo-container">
            <img class="logo" alt="Team achieve" src="../assets/logo.png" />
        </div>
        <img class="hero" alt="illustration" src="../assets/hero-image.png" />
        <div class="text">
            <h2>Team Achieve</h2>
            <p>Your perfect solution for funding your desires</p>
        </div>
    </div>
    <form class="right">
        <div class="form-header">
            <h1 class="welcome-back">Welcome Back</h1>
            <p>Enter your email address and password to access your account.</p>
        </div>
        <div class="form-group">
            <label for="email">Email Address<span class="required"> *</span></label>
            <input class="form-input" type="email" id="email" name="email" required />
        </div>
        <div class="form-group">
            <label for="password">Password<span class="required"> *</span></label>
            <input class="form-input" type="password" id="password" name="password" required />
        </div>
        <div class="sub-options" >
            <div>
                <input type="checkbox" id="remember" name="remember" />
                <label for="remember">Remember Me</label>
            </div>
            <a class="forgot-password" href="#">Forgot Password?</a>
        </div>
        <button class="login-button" type="submit">Login</button>
        <p>Don't have an account? <a class="sign-up" href="#">Sign Up</a></p>
    </form>
    
  </main>
</template>

<style scoped>
.login-layout {
    display: flex;
    justify-content: space-between;
    position: relative;
    width: 100%;
    height: 100vh; 
    overflow: hidden;
}
.logo {
  display: block;
    width: 198px;
    max-width: 30vw;
    padding-left: 20px;
}
.logo-container {
    display: flex;
    position: absolute;
    top: 16px;
    left: 16px;
    margin-right: 0;
    z-index: 20;
}
.left {
    display: flex;
    flex-direction: column;
    background-color: #F8EAFF;
    height: 100vh;
    align-items: center;
    width: 50%;
    border-top-right-radius: 20px;
    border-bottom-right-radius: 20px;
}
.right {
    display: flex;
    flex-direction: column;
    background-color: #FFFFFF;
    height: 100vh;
    align-items: center;
    margin-top: 0;
    justify-content: center; 
    width: 50%;
}

@media (max-width: 640px) {
    .login-layout {
        display: flex;
        flex-direction: column;
    }
    .right {
        width: 80%;
        height: auto;
    }
    .left{
        display: none;
    }
    .logo-container {
        position: static;
        margin: 16px auto;
    }
    .form-input, .login-button, .sub-options {
        width: calc(100% - 40px);
    }
    .right {
        margin-top: 24px;
    }
}
.text{
    display: flex;
    flex-direction: column;
    margin-top: 50px;
    align-items: center;
}
.form-header {
    display: flex;
    flex-direction: column;
    align-items: center;
    margin-bottom: 30px;
}
.right{
    background-color: #FCFCFC;
}
.form-input {
    display: block;
    width: 620px;
    height: 48px;
    margin-bottom: 20px;
    border: 1px solid #ccc;
    border-radius: 5px;
    padding: 2px 10px;
}
.required {
    color: red;
}
.form-group {
    display: flex;
    flex-direction: column;
    margin-bottom: 15px;
    gap: 5px;
}
.sub-options {
    display: flex;
    justify-content: space-between;
    width: 620px;
    margin-bottom: 20px;
}
.login-button {
    width: 620px;
    height: 48px;
    background-color: #61227D;
    color: white;
    border: none;
    border-radius: 5px;
    cursor: pointer;
}
.welcome-back {
    color: #61227D;
}
.hero {
    margin-top: 200px;
    border-radius: 15px;
}
.sign-up {
    color: #61227D;
    text-decoration: none;
    font-weight: bold;
}
.forgot-password {
    color: #61227D;
    text-decoration: none;
    font-weight: bold;
}
</style>