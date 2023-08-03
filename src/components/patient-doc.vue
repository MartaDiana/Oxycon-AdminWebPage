<template>
  <div class="container-patient-doc">
    <div class="dashboard section">
      <div class="row all-content">
        <!-- list -->
        <div class="col-lg-2 col-md-2 col-sm-4 list">
          <div class="row icon-dash">
            <div class="col">
              <img src="img/logo.png" alt="" />
              <span>Oxycon</span>
            </div>
          </div>
          <hr />
          <div class="all-list">
            <div class="row patient">
              <div class="col">
                <a href="patientlist.html">
                  <h6 class=""><span class="fa fa-wheelchair" style="font-size: 20px"></span>&nbsp;Patient</h6>
                </a>
              </div>
            </div>
            <hr />
            <div class="row doctor">
              <div class="col">
                <a href="doctorlist.html">
                  <h6><span class="fa fa-user-md" style="font-size: 20px"></span>&nbsp;Doctor</h6>
                </a>
              </div>
            </div>
            <hr />
            <div class="row tool">
              <div class="col">
                <a href="oxyconlist.html">
                  <h6><span class="fa fa-medkit" style="font-size: 20px"></span> Oxycon</h6>
                </a>
              </div>
            </div>
            <hr />
            <div class="d-flex justify-content-center">
              <button class="btn logout" id="logout">Log Out</button>
            </div>
          </div>
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
                <th>Nama Pasien</th>
                <th>ID Dokter Penangan</th>
                <th>Phone</th>
                <th>Email</th>
                <th>Device</th>
                <th>Action</th>
              </thead>
              <tbody id="pasienList"></tbody>
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
                <button id="Delpas" class="Delpas btn btn-danger" type="button">Delete Data</button>
              </div>
            </div>
          </div>
        </div>
        <!-- end of modal -->
      </div>
    </div>
  </div>
</template>
