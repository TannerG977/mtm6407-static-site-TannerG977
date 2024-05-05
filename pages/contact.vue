<template>
    <body class="bg">
      <h1 class="ms-5 mt-3">Contact</h1>
      <div class="containerdiv mt-5 shadow-lg">
        <form class="emailform" @submit.prevent="submitForm">
        <div class="form-group">
            <label for="exampleFormControlInput1">Full Name</label>
            <input type="text" class="form-control" id="exampleFormControlInput1" name="name" v-model="form.name" placeholder="John Doe">
            <label class="labelstyle" for="exampleFormControlInput1">Email address</label>
            <input type="email" class="form-control" id="exampleFormControlInput1" name="email"  v-model="form.email" placeholder="name@email.com">
        </div>
        <div class="form-group">
            <label class="labelstyle" for="exampleFormControlTextarea1">Your Message</label>
            <textarea class="form-control" id="exampleFormControlTextarea1" rows="3" name="message" v-model="form.message"></textarea>
        </div>
        <button class="submitbtn btn btn-primary" type="submit" @click="sent">Send Message</button>
        </form>
      </div>

        <div class="contact-info text-center">
            <p>Email: tannerg977@gmail.com</p>
            <p>GitHub: <a href="https://github.com/TannerG977">TannerG977</a></p>
            <p class="mb-5">LinkedIn: <a href="https://www.linkedin.com/in/tanner-green-02391a2a8/">Tanner Green</a></p>
        </div>
    </body>
  </template>


<script setup>
import { ref } from 'vue';

const form = ref({
  access_key: "6bf4b320-6577-401d-9bbf-29e1fd67b7b6",
  subject: "New Submission from Web3Forms",
  name: "",
  email: "",
  message: "",

});

const result = ref("");
const status = ref("");

const submitForm = async () => {
  result.value = "Please wait...";
  try {
    const response = await $fetch('https://api.web3forms.com/submit', {
      method: 'POST',
      headers: { 'Content-Type': 'application/json' },
      body: form.value,
    });

    console.log(response); // You can remove this line if you don't need it

    result.value = response.message;

    if (response.status === 200) {
      status.value = "success";
    } else {
      console.log(response); // Log for debugging, can be removed
      status.value = "error";
    }
  } catch (error) {
    console.log(error); // Log for debugging, can be removed
    status.value = "error";
    result.value = "Something went wrong!";
  } finally {
    // Reset form after submission
    form.value.name = "";
    form.value.email = "";
    form.value.message = "";

    // Clear result and status after 5 seconds
    setTimeout(() => {
      result.value = "";
      status.value = "";
    }, 5000);
  }
};

//Message Confirmation
function sent(event) {
  alert(`Message Sent`)
}
</script>

<style lang="css" scoped>

    body {
        padding-top: 50px;
    }

    .bg {
        background-image: url("/assets/background.png") !important;
        background-size: cover;
        background-attachment: fixed;
        background-position: center;
        height: 100vh;
        width: 100vw;
    }

    .emailform {
        margin-left: 10%;
        margin-right: 10%;
    }

    .labelstyle {
        margin-top: 15px;
    }

    .submitbtn {
        margin-top: 20px;
    }

    .btn-primary {
    background-color: #c4e2bc !important;
    color: black;
    margin-right: 12px !important;
    margin-top: 20px;
    }

    .btn-primary:hover {
        background-color: #688665 !important;
        color: white !important;
    }

    .contact-info {
        margin-top: 50px;
    }

    .containerdiv {
    border: solid #688665 10px;
    border-radius: 10px;
    margin-left: 20%;
    margin-right: 20%;
    background-color: white;
    padding-top: 20px;
    padding-bottom: 20px;
}

@media only screen and (max-width: 700px){
  
  .containerdiv {
      margin-left: 5%;
      margin-right: 5%;
  }


}
</style>