<template>
  <div class="container">
      <ul class="nav nav-tabs"  id="mainTab" role="tablist">
        <li class="nav-item" role="presentation">
          <button class="nav-link active" id="sasu-tab" data-bs-toggle="tab" data-bs-target="#sasu" type="button" role="tab" aria-controls="sasu" aria-selected="true">SASU</button>
        </li>
        <li class="nav-item" role="presentation">
          <button class="nav-link " id="eurl-tab" data-bs-toggle="tab" data-bs-target="#eurl" type="button" role="tab" aria-controls="eurl" aria-selected="true">EURL</button>
        </li>
        <li class="nav-item" role="presentation">
          <button class="nav-link " id="portage-tab" data-bs-toggle="tab" data-bs-target="#portage" type="button" role="tab" aria-controls="portage" aria-selected="true">Portage Salarial</button>
        </li>
        <li class="nav-item" role="presentation">
          <button class="nav-link " id="autoentrepreneur-tab" data-bs-toggle="tab" data-bs-target="#autoentrepreneur" type="button" role="tab" aria-controls="autoentrepreneur" aria-selected="true">Auto/Micro Entreprise</button>
        </li>
        <li class="nav-item" role="presentation">
          <button class="nav-link " id="employee-tab" data-bs-toggle="tab" data-bs-target="#employee" type="button" role="tab" aria-controls="employee" aria-selected="true">Salariat</button>
        </li>
      </ul>
      <div class="tab-content" id="mainTabContent">
        <div class="tab-pane fade show active" id="sasu" role="tabpanel" aria-labelledby="sasu-tab"><sasu-tab/></div>
        <div class="tab-pane fade" id="eurl" role="tabpanel" aria-labelledby="eurl-tab"><eurl-tab/></div>
        <div class="tab-pane fade" id="employee" role="tabpanel" aria-labelledby="salariat-tab"><employee-tab/></div>
        <div class="tab-pane fade" id="portage" role="tabpanel" aria-labelledby="salariat-tab"><portage-tab/></div>
        <div class="tab-pane fade" id="autoentrepreneur" role="tabpanel" aria-labelledby="autoentrepreneur-tab"><auto-entrepreneur-tab/></div>
      </div>
  </div>
</template>

<script>
import sasuTab from './SASUTab.vue'
import eurlTab from './EURLTab.vue'
import employeeTab from './EmployeeTab.vue'
import portageTab from './Portage.vue'
import autoEntrepreneurTab from './AutoEntrepreneurTab.vue'

export default {
  name: 'MainTab',
  components: {
    sasuTab, eurlTab, employeeTab, portageTab, autoEntrepreneurTab
  }
}
</script>

<style scoped>
li {
  margin: 0 10px;
}
</style>
