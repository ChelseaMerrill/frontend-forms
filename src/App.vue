
<script setup lang="ts">

</script>

<template>
  <CContainer>
    <CRow class="bill-form-row">
      <CCol>
        <h3>Compare Two versions of the same Bill</h3>
        <div class="bill-form-col">
          <div class="version-field">
            <p>First Version</p>
            <input/>
          </div>
          <div class="version-field">
            <p>Second Version</p>
            <input/>
          </div>
          <button class="compare-button">Compare</button>
        </div>
      </CCol>

      <CCol>
        <h3>Compare different Bills and Sessions</h3>
        <div class="bill-form-col">
          <div class="bill-group">
            <p>First Bill</p>
            <div class="bill-input-row"><p>Bill:</p><input/></div>
            <div class="bill-input-row"><p>Version:</p><input/></div>
            <div class="bill-input-row"><p>Session:</p><input/></div>
          </div>
          <div class="bill-group">
            <p>Second Bill</p>
            <div class="bill-input-row"><p>Bill:</p><input/></div>
            <div class="bill-input-row"><p>Version:</p><input/></div>
            <div class="bill-input-row"><p>Session:</p><input/></div>
          </div>
          <button class="compare-button">Compare</button>
        </div>
      </CCol>
    </CRow>
  </CContainer>
</template>


<style src="bootstrap/dist/css/bootstrap.min.css"></style>
<style>
.bill-form-row {
  display: flex;
  justify-content: space-between;
  text-align: center;
  font-family: Arial, Helvetica, sans-serif;
}
.bill-form-col {
  border: 2px solid rgb(48, 48, 48);
  height: 500px;
  width: 600px;
  border-radius: 5px;
  background-color: rgb(180, 216, 251);
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: space-between;
  padding-top: 50px;
  padding-bottom: 50px;
}
.compare-button{
  background-color: black;
  color: white;
  width: 200px;
  border: 2px white;
  border-radius: 5px;
}
.bill-input-row{
  display: flex;
  justify-content: space-between;
  align-items: baseline;
}

</style>