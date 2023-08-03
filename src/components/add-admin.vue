<template>
  <navbar />
  <!-- main content -->
  <div class="col-lg-12 col-md-12 col-sm-12 main">
    <div class="row">
      <div class="col title">
        <h1>ADD NEW USER ADMIN</h1>
        <p>A new admin will be added by filling in the form below.</p>
      </div>
    </div>
    <form class="sigup-form">
      <div class="form-group">
        <label for="exampleInputEmail1" style="color: rgb(216, 216, 216)">Name</label>
        <input type="text" class="form-control" id="exampleInputEmail1" aria-describedby="emailHelp" />
      </div>
      <div class="form-group">
        <label for="email-signup" style="color: rgb(216, 216, 216)">Email</label>
        <input type="email" class="form-control" id="email-signup" name="email" />
      </div>
      <div class="form-group">
        <label for="pass-signup" style="color: rgb(216, 216, 216)">Password</label>
        <input type="password" class="form-control" id="pass-signup" name="password" />
      </div>
      <div class="button text-center mt-3">
        <button class="btn submit-btn" style="margin-top: 10px">Sign Out</button>
      </div>
    </form>
  </div>
  <!-- end of main content -->

  <fot />
</template>

<script setup>
import fot from "./footer.vue";
import navbar from "./navbar.vue";
</script>

<style scoped>
.sigup-form {
  max-width: 21em;
  background-color: rgba(184, 220, 255, 0.3);
  margin: auto;
  border-radius: 15px;
  color: white;
  padding: 30px 30px;
  margin-bottom: 50px;
  margin-top: 50px;
  display: flex;
  flex-direction: column;
  gap: 10px;
}
label {
  margin-bottom: 5px;
}

.submit-btn {
  padding: 5px 28px;
  background-color: rgb(204, 204, 204);
}
</style>
