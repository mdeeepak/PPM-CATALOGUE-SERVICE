<template>
<div class="accordion" id="acordianForm">
  <div class="card">
    <div class="card-header" id="headingOne">
      <h2 class="mb-0">
        <button class="btn btn-link" type="button" data-toggle="collapse" data-target="#collapseOne" aria-expanded="true" aria-controls="collapseOne">
          {{accessData.title}}
        </button>
      </h2>
    </div>

    <div id="collapseOne" class="collapse show" aria-labelledby="headingOne" data-parent="#acordianForm">
      <div class="card-body">
        <form>
  <div class="form-group">
    <label for="dropDownSelect">{{accessData.dropDownSelect.name}}</label>
    <select class="form-control" id="dropDownSelect">
     <option v-for="optionIndex in accessData.dropDownSelect.options.length" :key="optionIndex">
       {{accessData.dropDownSelect.options[optionIndex-1]}}
     </option>
    </select>
  </div>
  <div class="form-group">
    <label for="grantText">{{grantText.name}}</label>
    <input type="text" class="form-control" id="grantText" placeholder="Enter grant text">
  </div>
  <div class="form-group">
    <label for="roSelect">{{ROSelect.name}}</label>
    <select class="form-control" id="roSelect">
      <option v-for="optionIndex in ROSelect.options.length" :key="optionIndex">
       {{ROSelect.options[optionIndex-1]}}
     </option>
    </select>
  </div>
</form>
      </div>
    </div>
  </div>
</div>
</template>


<script>
import optionData from '../../data/commonOptionJson.js' 
export default {
  props:['accessData'],
  data:function(){
    return optionData
  }
}
</script>
