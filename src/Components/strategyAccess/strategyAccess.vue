<template>
<div class="accordion" id="strategyAccessAccordian">
  <div class="card">
    <div class="card-header" id="headingOne">
      <h2 class="mb-0">
        <button class="btn btn-link" type="button" data-toggle="collapse" data-target="#collapseOne" aria-expanded="true" aria-controls="collapseOne">
          Strategy Access Required
        </button>
      </h2>
    </div>

    <div id="collapseOne" class="collapse show" aria-labelledby="headingOne" data-parent="#strategyAccessAccordian">
      <div class="card-body">
        <form>
  <div class="form-group">
    <label for="projectLevelSelect">Project Level</label>
    <select class="form-control" id="projectLevelSelect">
      <option>Select Project Level</option>
      <option>Organiztion</option>
      <option>Department</option>
      <option>Group</option>
      <option>Team/Product</option>
      <option>Project</option>
    </select>
  </div>
  <div class="form-group">
    <label for="grantDescription">Grant Description</label>
    <input type="text" class="form-control" id="grantDescription" placeholder="Enter grant description">
  </div>
  <div class="form-group">
    <label for="rorwgrants">RO/RW Grants</label>
    <select class="form-control" id="rorwgrants">
      <option>Select Grant Option </option>
      <option>RO</option>
      <option>RW</option>
    </select>
  </div>
</form>
      </div>
    </div>
  </div>
</div>
</template>