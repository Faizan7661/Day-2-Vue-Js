<script setup>
import { ref } from 'vue';

const details = ref({
  id: 1624,
  employeeName: "Mohammed Faizan",
  email: "faizan.500apps@gmail.com",
  designation: "Developer",
  mobileNumber: 7661936118
});
</script>

<template>
  <div class="container">
    <div class="card">
      <img src="https://my.ap1.500apps.com/pcors?url=https://ap1-infinity-user-data.s3.amazonaws.com/13416/avatars/494333/494333/117passportsizephoto-1.png" alt="Profile Picture">
      <h1>{{ details.employeeName }}</h1>
      <h2>Employee ID: {{ details.id }}</h2>
      <h2>Email: {{ details.email }}</h2>
      <h2>Designation: {{ details.designation }}</h2>
      <h2>Mobile Number: {{ details.mobileNumber }}</h2>
    </div>
  </div>
</template>



<style scoped>
.container {
  display: flex;
  justify-content: center;
  align-items: center;
  height:  100vh;
}

.card {
  width:  400px; 
  height:  500px; 
  padding:  20px;
  background-color: rgb(239,  248,  255);
  border-radius:  8px;
  box-shadow:  0  2px  4px rgba(0,  0,  0,  0.1);
  text-align: center;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  margin-left : 400px
}

.card img {
  width:  100px;
  height:  100px;
  border-radius:  50%;
  object-fit: cover;
  margin-bottom:  20px;
}

.card h1 {
  margin:  0;
  font-size:  2em; /* Increase font size */
  color: #12263f;
  font-weight: bold; /* Make text bold */
}

.card h2 {
  margin:  5px  0;
  font-size:  1.2em; /* Increase font size */
  color: #666;
  font-weight: normal; /* Make text normal weight */
}

</style>
