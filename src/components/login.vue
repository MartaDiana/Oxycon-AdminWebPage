<template>
  <div class="container-login">
    <div class="container homepage">
      <div class="row">
        <div class="col">
          <h4>Admin Login</h4>
          <p>Please enter your details to get sign!</p>
        </div>
      </div>
      <div class="row">
        <div class="col">
          <form class="login-form">
            <label for="email-login" style="color: rgb(216, 216, 216)">Email address</label>
            <input type="email" class="form-control" id="email-login" aria-describedby="emailHelp" name="email" />
            <label for="password-login" style="color: rgb(216, 216, 216)">Password</label>
            <input type="password" class="form-control" id="password-login" name="password" />
            <button type="submit" class="btn signin">Sign In</button>
          </form>
        </div>
      </div>
    </div>
    <div class="row signup">
      <div class="col">
        <p>Don't Have Account?</p>
        <a href="tambahadmin.html" target="_blank"> Create Account </a>
      </div>
    </div>
  </div>
</template>

<style scoped>
.container-login {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  font-family: "Poppins", sans-serif !important;
}
.homepage {
  max-width: 22em;
  width: 100%;
  background-color: rgba(184, 220, 255, 0.3);
  border-radius: 15px;
  color: white;
  padding: 40px;
  margin-bottom: 20px;
  margin-top: 50px;
}
.container h4 {
  color: rgb(216, 216, 216);
  text-align: center;
  margin: 15px 0;
  font-weight: 600;
  letter-spacing: 1.5px;
}

.col p:nth-child(2) {
  color: rgb(185, 185, 185);
  text-align: center;
  font-weight: 400;
}

.login-form {
  display: flex;
  flex-direction: column;
  gap: 10px;
}

.login-form button {
  margin-top: 30px;
}

.signin {
  margin: auto;
  background-color: rgb(216, 216, 216);
  border-radius: 10px;
  padding: 8px 40px;
}

.signup {
  /* background-color: black; */
  text-align: center;
}

.signup p:first-child {
  font-size: 0.9em;
  color: rgb(216, 216, 216);
  margin-bottom: 1px;
}

.signup a {
  text-decoration: none;
  font-size: 0.7em;
  color: rgb(216, 216, 216);
}

/* hover */

.signup a:hover {
  color: white;
}

/* end of hover */
</style>
