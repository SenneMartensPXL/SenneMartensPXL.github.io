<template>
  <div class="login">
    <h1>Login</h1>
    <div class="loginForm">
      <div class="loginFormItem">
        <label for="Username">Username</label>
        <input name="Username">
      </div>
      <div class="loginFormItem">
        <label for="Password">Password</label>
        <input type="password" name="Password">
      </div>
      <button class="button" type="button" value="Login" name="Login">Login</button>
    </div>
  </div>
</template>

<style>
.login {
  background-color: #343434;
  padding: 20px;
  border-radius: 10px;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  max-width: 500px;
  width: 100%;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}

h1 {
  text-align: center;
  color: #f2f2f2;
  margin-bottom: 20px;
  font-size: 24px;
}

.loginForm {
  display: flex;
  flex-direction: column;
}

.loginFormItem {
  display: flex;
  flex-direction: column;
  margin-bottom: 15px;
}

.loginFormItem label {
  margin-bottom: 5px;
  font-weight: bold;
  color: #f2f2f2;
}

input {
  padding: 10px;
  border-radius: 5px;
  border: 1px solid #ccc;
  font-size: 16px;
  width: 100%;
}

button {
  display: flex;
  justify-content: center;
  margin-top: 20px;
  background-color: #216477;
  color: white;
  padding: 10px 20px;
  border: none;
  border-radius: 5px;
  cursor: pointer;
  font-size: 16px;
}

button:hover {
  background-color: #025669;
}

@media (min-width: 768px) {
  .login {
    padding: 40px;
  }

  h1 {
    font-size: 28px;
  }

  input {
    font-size: 18px;
  }

  button input {
    padding: 12px 24px;
    font-size: 18px;
  }
}
</style>

<script>
</script>
