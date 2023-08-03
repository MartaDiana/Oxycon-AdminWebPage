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
          <h1>ADD NEW DOCTOR</h1>
          <p>Create a new doctor and add them to this site.</p>
        </div>
      </div>

      <form class="add pagetambahdokter">
        <div class="form-group">
          <label for="email" style="color: rgb(216, 216, 216)">Nama Dokter</label>
          <input type="text" class="form-control" id="email" aria-describedby="emailHelp" name="nama" required />
        </div>
        <div class="form-group">
          <label for="specialist" style="color: rgb(216, 216, 216)">Spesialisasi</label>
          <input type="text" class="form-control" id="specialist" name="specialist" required />
        </div>
        <div class="form-group">
          <label for="phone" style="color: rgb(216, 216, 216)">Phone</label>
          <input type="text" class="form-control" id="phone" name="phone" required />
        </div>
        <div class="form-group">
          <label for="alamat" style="color: rgb(216, 216, 216)">Address</label>
          <input type="text" class="form-control" id="alamat" name="alamat" required />
        </div>
        <div class="form-group">
          <label for="dokterid" style="color: rgb(216, 216, 216)">Dokter ID</label>
          <input type="text" class="form-control" id="dokterid" name="userId" required />
        </div>
        <div class="form-group">
          <label for="status" style="color: rgb(216, 216, 216)">Dokter Status: </label>
          <select name="status" id="status">
            <option value="active">Active</option>
            <option value="nonactive">Non active</option>
          </select>
        </div>
        <div class="button text-center">
          <button type="submit" class="btn submit-btn" style="margin-top: 10px">Submit</button>
        </div>
      </form>
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
.pagetambahdokter {
  max-width: 21em;
  background-color: rgba(184, 220, 255, 0.3);
  margin: auto;
  border-radius: 15px;
  color: white;
  padding: 30px 30px;
  margin-top: 10px;
  margin-bottom: 100px;
  display: flex;
  flex-direction: column;
  gap: 20px;
}

.form-group select {
  border-radius: 4px;
  min-width: 100%;
  padding: 6px;
}

label {
  margin-bottom: 5px;
}

select:focus {
  outline: none;
}
.submit-btn {
  padding: 5px 28px;
  background-color: rgb(204, 204, 204);
}

.footer {
  background-color: rgb(255, 255, 255);
  color: black;
}
</style>
