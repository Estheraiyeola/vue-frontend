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
      <div class="mobile-logo">
        <img class="logo" alt="Team achieve" src="../assets/logo.png" />
      </div>

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

      <div class="sub-options">
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
  width: 100%;
  height: 100vh;
  overflow: hidden;
}

.left {
  display: flex;
  flex-direction: column;
  background-color: #f8eaff;
  height: 100vh;
  align-items: center;
  width: 50%;
  border-top-right-radius: 20px;
  border-bottom-right-radius: 20px;
}

.logo-container {
  position: absolute;
  top: 16px;
  left: 16px;
}

.logo {
  width: 180px;
  max-width: 40vw;
}

.hero {
  margin-top: 200px;
  border-radius: 15px;
}

.text {
  display: flex;
  flex-direction: column;
  margin-top: 50px;
  align-items: center;
}

.right {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  background-color: #fcfcfc;
  width: 50%;
  padding: 2rem;
}

.form-header {
  text-align: center;
  margin-bottom: 30px;
}

.form-group {
  display: flex;
  flex-direction: column;
  margin-bottom: 15px;
  width: 100%;
  max-width: 620px;
}

.form-input {
  height: 48px;
  padding: 0 10px;
  border: 1px solid #ccc;
  border-radius: 5px;
}

.required {
  color: red;
}

.sub-options {
  display: flex;
  justify-content: space-between;
  width: 100%;
  max-width: 620px;
  margin-bottom: 20px;
}

.login-button {
  width: 100%;
  max-width: 620px;
  height: 48px;
  background-color: #61227d;
  color: white;
  border: none;
  border-radius: 5px;
  cursor: pointer;
}

.login-button:hover {
  background-color: #4b1762;
}

.welcome-back {
  color: #61227d;
}

.sign-up,
.forgot-password {
  color: #61227d;
  text-decoration: none;
  font-weight: bold;
}

.mobile-logo {
  display: none;
  margin-bottom: 1.5rem;
}

@media (max-width: 768px) {
  .login-layout {
    flex-direction: column;
    align-items: center;
    height: auto;
  }

  .left {
    display: none; 
  }

  .right {
    width: 90%;
    padding: 2rem 1rem;
    height: auto;
  }

  .form-input,
  .login-button,
  .sub-options {
    width: 100%;
  }

  .mobile-logo {
    display: flex;
    justify-content: center;
  }

  .logo {
    width: 150px;
  }

  .form-header h1 {
    font-size: 1.8rem;
  }

  .form-header p {
    font-size: 0.95rem;
  }
}
</style>
