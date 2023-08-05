<template>
  <div class="app">
    <JobList :jobList="jobList"></JobList>
  </div>
</template>

<script lang="ts">
import { defineComponent, reactive, ref, toRefs } from 'vue';
import JobList from './components/JobList.vue'
import Job from './models/Job'

export default defineComponent({
  name: 'App',
  components: {JobList},
  setup() {
    const jobList = ref<Job[]>([
      {title: 'AEM Developer', location: '4 Mohakhali', salary: 60000, id: 'aem_123'},
      {title: 'Java Developer', location: '2 Mohakhali', salary: 50000, id: 'java_124'},
      {title: 'Moodle Developer', location: 'Mirpur 12', salary: 45000, id: 'lms_125'},
    ])

    return {jobList}
  },
  methods: {
    
  }
});
</script>

<style>

</style>