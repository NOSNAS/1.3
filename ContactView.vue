<template>
    <div class="w3-padding-64 w3-content w3-text-grey" id="contact">
      <h2 class="w3-text-light-grey">Contact Me</h2>
      <hr style="width: 200px" class="w3-opacity">
  
      <div class="w3-section">
        <!-- contact -->
        <p><i class="fa fa-map-marker fa-fw w3-text-white w3-xxlarge w3-margin-right"></i> VICTORIA, AUS</p>
        <p><i class="fa fa-phone fa-fw w3-text-white w3-xxlarge w3-margin-right"></i> Phone: +61 123456</p>
        <p><i class="fa fa-envelope fa-fw w3-text-white w3-xxlarge w3-margin-right"></i> Email: mail@mail.com</p>
      </div><br>
  
      <!-- Form -->
      <form @submit.prevent="submitForm">
        <div class="w3-section">
          <label for="name">Name</label>
          <input type="text" id="name" v-model="formData.name" required>
        </div>
        <div class="w3-section">
          <label for="email">Email</label>
          <input type="email" id="email" v-model="formData.email" required>
        </div>
        <div class="w3-section">
          <label for="message">Message</label>
          <textarea id="message" v-model="formData.message" required></textarea>
        </div>
        <button type="submit" class="w3-button w3-black">Submit</button>
      </form>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        formData: {
          name: '',
          email: '',
          message: ''
        }
      };
    },
    methods: {
      submitForm() {
        // Handle form submission 
        console.log('Form data:', this.formData);
        
      }
    }
  };
  </script>
  
  <style scoped>
  form {
  max-width: 400px;
  margin: 0 auto;
}

label {
  display: block;
  font-weight: bold;
  margin-bottom: 6px;
}

input[type="text"],
input[type="email"],
textarea {
  width: 100%;
  padding: 10px;
  margin-bottom: 20px;
  border: 1px solid #ccc;
  border-radius: 4px;
}

textarea {
  resize: vertical;
  height: 150px;
}

button[type="submit"] {
  background-color: #333;
  color: white;
  border: none;
  padding: 10px 20px;
  border-radius: 4px;
  cursor: pointer;
}

button[type="submit"]:hover {
  background-color: #111;
}

  </style>
  