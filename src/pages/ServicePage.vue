<template>
  <NavBar />
 <HomeWork/>
 <ExpertMedical :nurses="nursesData"/>
 <Footer></Footer>
</template>
<script setup>
import ExpertMedical from '@/components/ExpertMedical.vue';
import HomeWork from '@/components/HomeWork.vue';

import NavBar from '@/components/NavBar.vue';

import Footer from '@/components/Footer.vue';
import img1 from '@/assets/pexels-oys-photography-838143052-19438561-removebg-preview.png'
import img2 from '@/assets/pexels-tima-miroshnichenko-5407249-removebg-preview.png'
import img3 from '@/assets/pexels-konrads-photo-32254655-removebg-preview.png'
import img4 from '@/assets/pexels-konrads-photo-32160037-removebg-preview.png'
const nursesData = [
  {
    name: "Dr. John Williams",
    specialty: "Cardiology Specialist",
    img: img1,
  },
  {
    name: "Dr. Sarah Johnson",
    specialty: "Pediatric Care",
    img:img2,
  },
  {
    name: "Dr. Michael Chen",
    specialty: "General Health",
    img: img3,
  },
  {
    name: "Dr. James Anderson",
    specialty: "Emergency Care",
    img: img4,
  },
];
</script>
<style scoped>
.animationtransform {
  animation: translate 9s ease-in-out infinite;
}
@keyframes translate {
  0% {
    transform: translateY(15px);
  }
  50% {
    transform: translateY(0px);
  }
  100% {
    transform: translateY(15px);
  }
}
</style>
