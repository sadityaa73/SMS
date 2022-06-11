<template>
  <div id="MainContent">
    <div id="LeftContainer">
      <div class="Dashboard" @click="dashboardComp">
        <p>Dashboard</p>
      </div>
      <div class="Student" @click="studentComp">
        <p>Student</p>
      </div>
      <div class="Teacher" @click="teacherComp">
        <p>Teacher</p>
      </div>
      <div class="Admin" @click="adminComp">
        <p>Admin</p>
      </div>
    </div>
    <div id="RightContainer">
      <dashboardComp v-if="dashboard" />
      <StudentComp v-if="student" />
      <TeacherComp v-if="teacher" />
      <AdminComp v-if="admin" />
    </div>
  </div>
</template>
<script>
import dashboardComp from "../dashboard/dashboardComp.vue";
import StudentComp from "../student/StudentComp.vue";
import TeacherComp from "../teacher/TeacherComp.vue";
import AdminComp from "../Admin/AdminComp.vue";
export default {
  name: "mainCOntent",
  components: {
    dashboardComp,
    StudentComp,
    TeacherComp,
    AdminComp,
  },
  data() {
    return {
      dashboard: false,
      teacher: false,
      student: false,
      admin: false,
    };
  },
  methods: {
    studentComp() {
      this.student = !this.student;
      this.dashboard = false;
      this.teacher = false;
    },
    dashboardComp() {
      this.dashboard = !this.dashboard;
      this.student = false;
      this.teacher = false;
    },
    teacherComp() {
      this.teacher = !this.teacher;
      this.dashboard = false;
      this.student = false;
    },
    adminComp() {
      this.admin = !this.admin;
      this.teacher = false;
      this.dashboard = false;
      this.student = false;
    },
  },
};
</script>
<style scoped>
#MainContent {
  display: flex;
}
#LeftContainer {
  display: flex;
  flex-direction: column;
  border: 1px solid black;
  width: 20%;
  height: 80vh;
}
#RightContainer {
  display: flex;
  border: 1px solid black;
  width: 80%;
  height: 80vh;
}
.Dashboard {
  display: flex;
  border: 1px solid black;
  justify-content: center;
}
.Student {
  display: flex;
  border: 1px solid black;
  justify-content: center;
}
.Teacher {
  display: flex;
  border: 1px solid black;
  justify-content: center;
}
.Admin {
  display: flex;
  border: 1px solid black;
  justify-content: center;
}
</style>