
<script setup lang="ts">
const ArrayOne = [
    {
        pageLine: 'Page 1 Line 1',
        content: 'removedContent'
    },
    {
        pageLine: "Page 1 Line 3",
        content: 'this content was also removed'
    },
    {
        pageLine: "Page 2 Line 3",
        content: 'this content was also removed'
    }
]

const ArrayTwo = [
    {
        pageLine: 'Page 1 Line 5',
        content: 'It is a long established fact that a reader will be distracted by the readable content of a page when looking at its layout. The point of using Lorem Ipsum is that it has a more-or-less normal distribution of letters, as opposed to using'
    },
    {
        pageLine: "Page 5 Line 3",
        content: 'this content was added'
    },
    {
        pageLine: "Page 5 Line 4",
        content: 'It is a web page editors now use Lorem Ipsum as their default model text, and a search will uncover many web sites still in their infancy. Various versions have evolved over the years, sometimes by accident, sometimes on purpose (injected humour and the like).'
    }

]

</script>

<template>
  <CContainer>
    <CRow class="bill-form-row">
      <CCol>
        <h3>Compare Two versions of the same Bill</h3>
        <div class="bill-form-col">
          <div class="version-field">
            <span>First Version</span>
            <br/>
            <input/>
          </div>
          <div class="version-field">
            <span>Second Version</span>
            <br/>
            <input/>
          </div>
          <button class="compare-button">Compare</button>
        </div>
      </CCol>
      <CCol>
        <h3>Compare different Bills and Sessions</h3>
        <div class="bill-form-col">
          <div class="bill-group">
            <span>First Bill</span>
            <div class="bill-input-row"><p>Bill:</p><input/></div>
            <div class="bill-input-row"><p>Version:</p><input/></div>
            <div class="bill-input-row"><p>Session:</p><input/></div>
          </div>
          <div class="bill-group">
            <span>Second Bill</span>
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
        <span>Page 1 Line 15</span>
      </div>
      <div class="changed-text removed-text">
        <p>changedtext</p>
      </div>
    </div>
    <div class="diff-col diff-col-two">
      <div class="page-line-heading">
        <span>Page 2 Line 1</span>
      </div>
      <div class="changed-text added-text">
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
  vertical-align: middle;
  padding: 5px;
}
.page-line-heading span{
  padding-left: 5px;
  font-weight: 500;
}
.removed-text{
  color: red;
  text-decoration: line-through;
}
.added-text{
  color:blue;
  font-weight: 700;
}
.changed-text{
  padding: 10px;
}
</style>