<template>
    <body class="bg">
      <main>
      <div class="contactdiv mt-5 shadow-lg rounded-4" data-aos="fade-up" data-aos-duration="1000">
        <form class="emailform" @submit.prevent="submitForm">
        <div class="form-group">
            <label for="exampleFormControlInput1">Full Name</label>
            <input type="text" class="form-control" id="exampleFormControlInput1" name="name" v-model="form.name" placeholder="John Doe">
            <label class="labelstyle" for="exampleFormControlInput1">Email address</label>
            <input type="email" class="form-control" id="exampleFormControlInput1" name="email"  v-model="form.email" placeholder="name@email.com">
        </div>
        <div class="form-group">
            <label class="labelstyle" for="exampleFormControlTextarea1">Your Message</label>
            <textarea class="form-control" id="exampleFormControlTextarea1" rows="8" name="message" v-model="form.message"></textarea>
        </div>
        <button class="submitbtn button-18" type="submit" @click="sent">Send Message</button>
        </form>
        <div class="contact-info text-center rounded-bottom-4">
            <p>Email: tannerg977@gmail.com</p>
            <p>GitHub: <a href="https://github.com/TannerG977">TannerG977</a></p>
            <p>LinkedIn: <a href="https://www.linkedin.com/in/tanner-green-02391a2a8/">Tanner Green</a></p>
        </div>
      </div>
      </main>
    </body>
    <footer></footer>
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

    footer {
      height: 50px;
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
        padding-top: 20px;
        padding-bottom: 20px;
        background-color: #c4e2bc;
        margin-bottom: none !important;
    }

    .contactdiv {
    margin-left: 20%;
    margin-right: 20%;
    background-color: white;
    padding-top: 20px;
    margin-bottom: none !important;
}

.button-18 {
  align-items: center;
  background-color: #c4e2bc !important;
  border: 0;
  border-radius: 100px;
  box-sizing: border-box;
  color: black;
  cursor: pointer;
  display: inline-flex;
  font-size: 16px;
  font-weight: 600;
  justify-content: center;
  line-height: 20px;
  max-width: 480px;
  min-height: 40px;
  min-width: 0px;
  overflow: hidden;
  padding: 0px;
  padding-left: 20px;
  padding-right: 20px;
  text-align: center;
  touch-action: manipulation;
  transition: background-color 0.167s cubic-bezier(0.4, 0, 0.2, 1) 0s, box-shadow 0.167s cubic-bezier(0.4, 0, 0.2, 1) 0s, color 0.167s cubic-bezier(0.4, 0, 0.2, 1) 0s;
  user-select: none;
  -webkit-user-select: none;
  vertical-align: middle;
}

.button-18:hover { 
  background-color: #688665 !important;
  color: #ffffff;
}

@media only screen and (max-width: 700px){
  
  .contactdiv {
      margin-left: 5%;
      margin-right: 5%;
  }


}
</style>