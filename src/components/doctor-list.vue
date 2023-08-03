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
              <h1>DOCTOR LIST</h1>
            </div>
          </div>
          <div class="row">
            <div class="col buttonupdate">
              <a href="#">
                <button>
                  <span class="fa fa-plus-circle" style="font-size: 20px"></span>
                  Add New Doctor
                </button>
              </a>
            </div>
          </div>
          <br />
          <div class="doctorlist-title">
            <table class="table">
              <thead>
                <th>No.</th>
                <th>Nama Dokter</th>
                <th>Spesialisasi</th>
                <th>Alamat</th>
                <th>Phone</th>
                <th>Status</th>
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
                <h5 class="modal-title" id="exampleModalLabel">Update Data Dokter</h5>
                <button type="button" class="close" data-dismiss="modal" aria-label="Close">
                  <span aria-hidden="true">&times;</span>
                </button>
              </div>
              <div class="modal-body">
                <label for="" class="labs">Nama:</label>
                <input type="text" id="namadokter" /> <br />
                <label for="" class="labs">Spesialisasi:</label>
                <input type="text" id="spedokter" /> <br />
                <label for="" class="labs">Alamat:</label>
                <input type="text" id="aldokter" /> <br />
                <label for="" class="labs">Phone:</label>
                <input type="text" id="phodokter" /> <br />
                <label for="status" class="labs">Status:</label>
                <select name="status" id="status" style="width: 100%">
                  <option value="active">Active</option>
                  <option value="nonactive">Non active</option>
                </select>
                <label for="" class="labs" style="display: none">ID Dokument</label>
                <input type="text" id="iddocdok" style="display: none" />
                <br />
              </div>
              <div class="modal-footer">
                <button id="UpDatadoc" class="UpDatadoc btn btn-success" type="button">Update Data</button>
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
                <label for="namadokter" class="labs" style="display: none">Namaa:</label>
                <input type="text" id="namadokter" style="display: none" />
                <label for="spedokter" class="labs" style="display: none">Spesialisasi:</label>
                <input type="text" id="spedokter" style="display: none" />
                <label for="aldokter" class="labs" style="display: none">Alamat:</label>
                <input type="text" id="aldokter" style="display: none" />
                <label for="phodokter" class="labs" style="display: none">Phone:</label>
                <input type="text" id="phodokter" style="display: none" />
                <label for="" class="labs" style="display: none">ID Dokument</label>
                <input type="text" id="iddocdok" style="display: none" />
              </div>
              <div class="modal-btn">
                <button id="Deldoc" class="DelDoc btn btn-danger" type="button">Delete Data</button>
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

/* end of button */
.footer {
  background-color: rgb(255, 255, 255);
  color: black;
}
</style>
