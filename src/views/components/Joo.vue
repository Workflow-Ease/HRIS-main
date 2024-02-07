<template>
  <div class="card">
    <div class="p-3 pb-0 card-header">
      <div class="d-flex justify-content-between">
        <h6 class="mb-2">부서별 성과</h6>
      </div>
    </div>
    <div class="table-responsive">
      <table class="table text-center">
        <thead>
          <tr>
            <th>부서 이름</th>
            <th>부서 성과</th>
          </tr>
        </thead>
        <tbody>
          <tr v-for="(department, index) in uniqueDepartments" :key="index">
            <td class="text-center">{{ department.departmentName }}</td>
            <td class="text-center">{{ department.departmentPerformance }}</td>
          </tr>
        </tbody>
      </table>
    </div>
  </div>
</template>

<script>
export default {
  computed: {
    uniqueDepartments() {
      const unique = {};
      this.top5Departments.forEach(department => {
        unique[department.departmentName] = department;
      });
      return Object.values(unique);
    }
  }
}
</script>
