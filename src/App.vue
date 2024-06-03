<template>
  <div class="container">
    <div class="bg-image"></div>
    <div class="form-wrapper">
      <div class="form-header">
        <h2>Hey! One Last Step!</h2>
      </div>
      <form @submit.prevent="handleSubmit">
        <div class="form-group country">
          <label for="country">Country</label>
          <input type="text" id="country" v-model="formData.country" required>
        </div>
        <div class="form-group provider">
          <label for="provider">Provider</label>
          <input type="text" id="provider" v-model="formData.provider" required>
        </div>
        <div class="form-group remember-me">
          <input type="checkbox" id="rememberMe" v-model="formData.rememberMe">
          <label for="rememberMe">Remember Me</label>
        </div>
        <button type="submit" class="submit-btn">Submit</button>
      </form>
    </div>
    <div class="branding">
      <h1>Nokia</h1>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      formData: {
        country: '',
        provider: '',
        rememberMe: false
      }
    }
  },
  methods: {
    handleSubmit() {
      console.log(this.formData)
    }
  }
}
</script>

<style>
.container {
  display: flex;
  overflow: hidden;
  justify-content: center;
  align-items: center;
  height: 100vh;
  position: relative;
  overflow: hidden;
  background-color: none;
}

.bg-image {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-image: url('../public/nokia.png');
  background-attachment: fixed;
  background-size:  cover;
  background-position: center;
  opacity: 1;
  z-index: -1;
}


.form-wrapper {
  width: 50%;
  padding: 20px;
  background-color: white;
  border-radius: 20px;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
  opacity: 0.85;

}

.form-header {
  background-color: black;
  margin-bottom: 20px;
  color: #fff;
  padding: 10px;
  border-top-left-radius: 5px;
  border-top-right-radius: 5px;
  border-radius: 20px;
  
}

.branding {
  width: 30%;
  text-align: center;
  font-size: 48px;
  font-weight: bold;
  color: lightblue;
  font-style: nokkok;
}

.form-group {
  margin-bottom: 15px;
  display: flex;
  align-items: center;
  font-size: larger;
}

.remember-me {
  align-items: flex-start;
}

label {
  display: block;
  margin-right: 10px;
  font-weight: bold;
  margin-top: 0px;
  margin-bottom: 20px;
}

input[type="text"],
input[type="checkbox"] {
  padding: 8px;
  border: 1px solid #ccc;
  border-radius: 3px;
  width: 100%;
}

input[type="checkbox"] {
  width: auto;
  margin-right: 5px;
}

.submit-btn {
  margin-left: 80%;
  padding: 10px 20px;
  background-color: green;
  color: #fff;
  border: none;
  border-radius: 15px;
  cursor: pointer;
  
}

@media (max-width: 768px) {
  .container {
    flex-direction: column;
    height: auto;
  }

  .form-wrapper,
  .branding {
    width: 100%;
  }

  .branding {
    margin-top: 20px;
    font-size: 36px;
  }
}
</style>