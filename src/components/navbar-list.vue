<template>
  <div class="list">
    <div class="row icon-dash">
      <div class="col">
        <img src="./icons/logo.png" alt="" />
        <span>Oxycon</span>
      </div>
    </div>
    <div class="line" style="margin-bottom: 20px"></div>
    <div class="all-list">
      <div class="row patient">
        <div class="col">
          <a href="patientlist.html">
            <h4 class=""><span class="fa fa-wheelchair" style="font-size: 28px"></span>&nbsp;Patient</h4>
          </a>
        </div>
      </div>
      <div class="line"></div>
      <div class="row doctor">
        <div class="col">
          <a href="doctorlist.html">
            <h4><span class="fa fa-user-md" style="font-size: 28px"></span>&nbsp;Doctor</h4>
          </a>
        </div>
      </div>
      <div class="line"></div>
      <div class="row tool">
        <div class="col">
          <a href="oxyconlist.html">
            <h4><span class="fa fa-medkit" style="font-size: 28px"></span> Oxycon</h4>
          </a>
        </div>
      </div>
      <div class="line"></div>
      <div class="d-flex justify-content-center">
        <button class="btn logout" id="logout">Log Out</button>
      </div>
    </div>
  </div>
</template>

<style scoped>
.list {
  filter: grayscale(10%);
  background: linear-gradient(30deg, rgb(16, 12, 59), rgb(0, 122, 156));
  padding: 30px;
  min-height: 100vh;
}
.icon-dash {
  color: rgb(255, 255, 255);
  font-family: "Righteous", cursive;
  font-size: 1.5em;
  margin-bottom: 52px;
}

.icon-dash img {
  max-width: 2.3em;
  margin-right: 8px;
}

/* line */
.line {
  height: 0.5px;
  width: 100%;
  background-color: rgba(164, 164, 164, 0.4);
}

.all-list {
  display: flex;
  flex-direction: column;
  gap: 20px;
}

a {
  text-decoration: none;
  color: #f1f1f1;
}

h4 {
  display: flex;
  flex-wrap: wrap;
  /* justify-content: center; */
  gap: 10px;
  align-items: center;
  font-weight: 400;
  font-size: 1.1em;
}

a:hover,
h4:hover {
  color: grey;
}
.logout {
  margin-top: 50px;
  background-color: rgb(16, 141, 213);
  color: #f1f1f1;
  padding: 10px 30px;
}

.logout:hover {
  background-color: rgba(16, 141, 213, 0.767);
}
</style>
