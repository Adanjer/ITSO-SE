<template>
    <div class="page-wrapper">
  
      <!-- Content -->
      <div class="container">
        <div class="privacy-section">
          <h1>ITSO Privacy Statement</h1>
          <p>
            At ITSO, we respect your privacy and the value of your intellectual property. When you submit personal 
            information or intellectual property to us, we commit to handling it with care and confidentiality.
          </p>
        </div>
  
        <h2>Disclaimer</h2>
        <p>
          By submitting personal information or intellectual property to ITSO, you acknowledge that you have read and 
          understood our Privacy Statement. ITSO disclaims any liability for unauthorized access or misuse of your data 
          beyond our reasonable control. Use of our services implies your consent to our privacy practices as outlined.
        </p>
  
        <!-- Agree Button -->
        <button class="agree-button" @click="handleAgree">Agree</button>
      </div>
    </div>
  </template>
  
  <script setup>
  import { useRouter } from 'vue-router';
  
  const router = useRouter();
  
  const handleAgree = () => {
    console.log("User agreed to privacy statement");
    router.push("/ips1");
  };
  </script>
  
  <style scoped>
/* Reset and Global Styles */
body, html {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  height: 100%;
  background-color: white;
}
/* Page Wrapper */
.page-wrapper {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  min-height: 100vh;
  width: 100%;
  padding: 40px 20px;
}

/* Container */
.container {
  max-width: 800px;
  width: 100%;
  text-align: center; /* Ensures all content is centered */
  padding: 20px;
}

/* Headings */
h1, h2 {
  font-size: 20px;
  font-weight: bold;
  text-decoration: underline;
  text-align: center; /* Center-align headers */
}

h1 {
  color: #f596c6;
}

h2 {
  color: #b31b5e;
}

/* Paragraph */
p {
  font-size: 16px;
  line-height: 1.6;
  margin-bottom: 20px;
  text-align: center; /* Center text */
}

/* Disclaimer Text */
.privacy-section p {
  font-weight: normal;
}

/* Agree Button */
.agree-button {
  background-color: #d63384;
  color: white;
  font-size: 16px;
  padding: 12px 32px;
  border: none;
  border-radius: 20px;
  cursor: pointer;
  transition: background-color 0.3s;
  display: block;
  margin: 0 auto; /* Centers the button */
}

.agree-button:hover {
  background-color: #b31b5e;
}

</style>
