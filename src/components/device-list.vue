<template>
  <div class="row all-content">
    <!-- list -->
    <div class="col-lg-2 col-md-2 col-sm-4 list">
      <navbarList />
    </div>
    <!-- end of list -->

    <!-- main content -->
    <div class="col-lg-10 col-md-10 col-sm-8 main">
      <div class="row">
        <div class="col title">
          <h1>PRODUCT LIST</h1>
        </div>
      </div>
      <div class="row">
        <div class="col buttonupdate">
          <a href="#">
            <button>
              <span class="fa fa-plus-circle" style="font-size: 20px"></span>
              Add New Device
            </button>
          </a>
        </div>
      </div>
      <br />
      <div class="row oxyconlist">
        <div class="col-md-3 col-lg-3">
          <div class="card" style="width: 18rem">
            <img src="./pic/oxycon.png" class="card-img-top" />
            <ul class="list-group list-group-flush">
              <li class="list-group-item">Oxycon ID: 1976YQ</li>
              <li class="list-group-item">Spesification: -</li>
              <li class="list-group-item">Production Date: 8/8/2022</li>
            </ul>
            <div class="card-body text-center">
              <a href="#" class="card-link">Update</a>
              <span>&nbsp;|&nbsp;</span>
              <a href="#" class="card-link">Delete</a>
            </div>
          </div>
        </div>
      </div>
    </div>
    <!-- end of main content -->
  </div>
  <fot />
</template>

<script setup>
import fot from "./footer.vue";
import navbarList from "./navbar-list.vue";
</script>

<style scoped>
.oxyconlist img {
  max-width: 10em;
  margin: auto;
  padding: 5px;
}

.oxyconlist {
  margin-top: 50px;
  margin-left: 15px;
  margin-right: 15px;
}

.footer {
  background-color: rgb(255, 255, 255);
  color: black;
}

.card-link:hover {
  color: blue;
}
</style>
