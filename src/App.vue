
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

  <CContainer class="diff-container">
    <div class="diff-col diff-col-one">
      <div class="page-line-heading">
        <p>Page</p>
        <p>1</p>
        <p>Line</p>
        <p>1</p>
      </div>
      <div>
        <p>changedtext</p>
      </div>
    </div>
    <div class="diff-col diff-col-two">
      <div class="page-line-heading">
        <p>Page</p>
        <p>1</p>
        <p>Line</p>
        <p>1</p>
      </div>
      <div>
        <p>It is a long established fact that a reader will be distracted by the readable content of a page when looking at its layout. The point of using Lorem Ipsum is that it has a more-or-less normal distribution of letters, as opposed to using 'Content here, content here', making it look like readable English. Many desktop publishing packages and web page editors now use Lorem Ipsum as their default model text, and a search for 'lorem ipsum' will uncover many web sites still in their infancy. Various versions have evolved over the years, sometimes by accident, sometimes on purpose (injected humour and the like).</p>
      </div>
    </div>
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
.diff-container{
  margin-top: 50px;
  display: flex;
  justify-content: space-between;
}
.diff-col{
  border: 2px solid black;
  width: 600px;
}
.page-line-heading{
  display: flex;
  background-color: rgb(204, 211, 211);
}
.page-line-heading p{
  padding-left: 5px;
}

</style>