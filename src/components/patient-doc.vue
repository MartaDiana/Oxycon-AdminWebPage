<template>
  <div class="container-patient-doc">
    <div class="dashboard section">
      <div class="row all-content">
        <!-- list -->
        <div class="col-lg-2 col-md-2 col-sm-4">
          <navbarList />
        </div>
        <!-- end of list -->

        <!-- main content -->
        <div class="col-lg-10 col-md-10 col-sm-8 main">
          <div class="row">
            <div class="col title">
              <h1>PATIENT LIST</h1>
            </div>
          </div>
          <div class="doctorlist-title">
            <table class="table">
              <thead>
                <th>No.</th>
                <th>Name</th>
                <th>Referral Doctor</th>
                <th>Phone</th>
                <th>Email</th>
                <th>ID Device</th>
                <th>Action</th>
              </thead>
              <tbody>
                <tr></tr>
              </tbody>
              <!-- <tbody id="pasienList"></tbody> -->
            </table>
          </div>
        </div>
        <!-- end of main content -->

        <!-- Modal 1 -->
        <div class="modal fade" id="exampleModal1" tabindex="-1" aria-labelledby="exampleModalLabel" aria-hidden="true">
          <div class="modal-dialog modal-dialog-centered">
            <div class="modal-content">
              <div class="modal-header">
                <h5 class="modal-title" id="exampleModalLabel">Update Data Pasien</h5>
                <button type="button" class="close" data-dismiss="modal" aria-label="Close">
                  <span aria-hidden="true">&times;</span>
                </button>
              </div>
              <div class="modal-body">
                <label for="" class="labs">Nama:</label>
                <input type="text" id="namapasien" /> <br />
                <label for="" class="labs">Dokter:</label>
                <select name="" id="dokterList" style="width: 100%"></select>
                <!-- <input type="text" id="dokterpasien" />  -->
                <br />
                <label for="" class="labs">Phone:</label>
                <input type="text" id="phonepasien" /> <br />
                <label for="" class="labs">email:</label>
                <input type="text" id="emailpasien" /> <br />
                <label for="" class="labs" style="display: none">ID Dokumen</label>
                <input type="text" id="idpasien" style="display: none" />
                <br />
              </div>
              <div class="modal-footer">
                <button id="UpDataPas" class="UpDataPas btn btn-success" type="button">Update Data</button>
                <!-- <button id="Deldoc" class="DelDoc btn btn-danger" type="button">Delete Data</button> -->
              </div>
            </div>
          </div>
        </div>
        <!-- end of modal 1 -->
        <!-- Modal -->
        <div class="modal fade" id="exampleModal2" tabindex="-1" aria-labelledby="exampleModalLabel" aria-hidden="true">
          <div class="modal-dialog modal-dialog-centered">
            <div class="modal-content">
              <div class="modal-header">
                <h5 class="modal-title" id="exampleModalLabel">Are You Sure to Delete Data?</h5>
                <button type="button" class="close" data-dismiss="modal" aria-label="Close">
                  <span aria-hidden="true">&times;</span>
                </button>
              </div>
              <div class="modal-body">
                <label for="" class="labs" style="display: none">Nama:</label>
                <input type="text" id="namapasien" style="display: none" />
                <label for="" class="labs" style="display: none">Dokter:</label>
                <input type="text" id="dokterpasien" style="display: none" />
                <label for="" class="labs" style="display: none">Phone:</label>
                <input type="text" id="phonepasien" style="display: none" />
                <label for="" class="labs" style="display: none">email:</label>
                <input type="text" id="emailpasien" style="display: none" />
                <label for="" class="labs" style="display: none">ID Dokumen</label>
                <input type="text" id="idpasien" style="display: none" />
              </div>
              <div class="modal-btn">
                <button id="Delpas" class="Delpas" type="button">Delete Data</button>
              </div>
            </div>
          </div>
        </div>
        <!-- end of modal -->
      </div>
    </div>
  </div>
  <fot />
</template>

<script setup>
import fot from "./footer.vue";
import navbarList from "./navbar-list.vue";
</script>

<style scoped>
/* title and table */
.table {
  --bs-table-bg: none;
}

th {
  font-size: 1.2em;
  font-weight: 600;
}

td {
  font-weight: lighter;
}

th,
td {
  color: #f1f1f1;
}

.footer {
  background-color: rgb(255, 255, 255);
  color: black;
}
</style>
