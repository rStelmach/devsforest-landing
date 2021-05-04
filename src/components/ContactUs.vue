<template>
  <div id="contact" class="container">
    <header>Get In Touch!</header>
    <h1>Contact Us For a quote, help ot to join the team</h1>
    <section class="contact">
      <div>
        <img src="../images/phone.svg" alt="phone number" />
        <p>111 222 333</p>
      </div>
      <div class="frame">
        <img src="../images/mail.svg" alt="e-mail" />
        <p>info@example.com</p>
      </div>
      <div>
        <img src="../images/street.svg" alt="street" />
        <p>123 Street Block</p>
      </div>
    </section>
    <div class="form">
      <div class="wrapping">
        <form id="my-form" @submit.prevent="submitForm">
          <div class="wrapper">
            <div class="form-control" :class="{ invalid: !name.isValid }">
              <label for="yourname">Your Name</label>
              <input
                type="text"
                id="yourname"
                placeholder=" &#xf007;      Your Name"
                style="font-family:Poppins, FontAwesome"
                v-model.trim="name.value"
                @blur="clearValidity('name')"
              />
              <p v-if="!name.isValid">Please enter your name !</p>
            </div>
            <div class="form-control" :class="{ invalid: !email.isValid }">
              <label for="email"> Mail</label>
              <input
                type="email"
                id="email"
                placeholder="&#xf0e0;      your@email.com"
                style="font-family:Poppins, FontAwesome"
                v-model.trim="email.value"
                @blur="clearValidity('email')"
              />
              <p v-if="!email.isValid">Please enter correct e-mail !</p>
            </div>
            <div class="form-control " :class="{ invalid: !phone.isValid }">
              <label for="phone">Phone</label>
              <input
                type="text"
                id="phone"
                placeholder=" &#xf879;      Phone"
                style="font-family:Poppins, FontAwesome"
                v-model.number="phone.value"
                @blur="clearValidity('phone')"
              />
              <p v-if="!phone.isValid">Please enter your phone number !</p>
            </div>
          </div>
          <div class="message">
            <div class="form-control">
              <label for="message">Message</label>
              <textarea
                id="message"
                rows="12"
                placeholder="type here..."
                maxlength="500"
                style="font-family:Poppins, FontAwesome"
                v-model="message.value"
              />
            </div>
          </div>
        </form>
      </div>
      <div class="button"><button type="submit" form="my-form">Send message</button></div>
    </div>
  </div>
</template>

<script>
import { reactive, ref } from 'vue';
import axios from 'axios';

export default {
  setup() {
    const name = reactive({ value: '', isValid: true });
    const email = reactive({ value: '', isValid: true });
    const phone = reactive({ value: '', isValid: true });
    const message = reactive({ value: '', isValid: true });
    const formIsValid = ref(true);

    function clearValidity(input) {
      this[input].isValid = true;
    }
    function validateForm() {
      formIsValid.value = true;
      if (name.value === '') {
        name.isValid = false;
        formIsValid.value = false;
      }
      if (email.value === '') {
        email.isValid = false;
        formIsValid.value = false;
      }
      if (phone.value === '') {
        phone.isValid = false;
        formIsValid.value = false;
      }
    }
    function submitForm() {
      validateForm();
      if (!formIsValid.value) {
        return;
      }
      console.log(name.value, email.value, phone.value, message.value);
      axios.post('https://devs-test-d3a40-default-rtdb.europe-west1.firebasedatabase.app/messages.json', {
        name: name.value,
        email: email.value,
        phone: phone.value,
        message: message.value,
      });
      name.value = '';
      email.value = '';
      phone.value = '';
      message.value = '';
    }
    return { name, email, phone, message, formIsValid, submitForm, validateForm, clearValidity };
  },
};
</script>

<style lang="scss" scoped>
.container {
  max-width: 100vw;
  min-height: 120vh;
  background-color: #ffffff;
  header {
    text-align: center;
    color: black;
    font-size: 50px;
    font-weight: bold;
    padding-top: 5%;
  }
  h1 {
    font-size: 18px;
    color: black;
    text-align: center;
  }
  .contact {
    margin: 0 auto;
    display: flex;

    justify-content: space-between;

    width: 48%;
    padding: 2% 2%;
    .frame {
      border: 1px solid white;
      box-shadow: 5px 24px 50px -10px rgba(135, 135, 135, 0.19);
      border-radius: 10px;
      background-color: white;
    }
    div {
      width: 30%;
      margin-top: 1%;
      padding: 2% 0;

      img {
        display: block;
        margin: 0 auto;
      }
      p {
        text-align: center;
        margin-top: 10%;
        font-size: 16px;
        color: black;
      }
    }
  }
  .form {
    border: 1px solid #eaeaea;
    border-radius: 10px;
    margin: 0 auto;
    width: 65%;
    // display: flex;
    form {
      display: flex;
      flex-wrap: wrap;
      margin: 2% 5%;

      .form-control {
        margin: 0.5rem 0;
        width: 100%;

        label {
          display: block;
          font-size: 18px;
          font-weight: 500;
          margin-bottom: 0.5rem;
        }
        input,
        textarea {
          background-color: #f1f1f1;
          border: none;
          border-radius: 10px;
          font-size: 18px;
          width: 240%;
          min-height: 4rem;
          margin-bottom: 16%;
          resize: none;
          padding-left: 5%;
        }
      }
      .invalid {
        label {
          color: red;
        }
        input {
          border: 1px solid red;
        }
        ::-webkit-input-placeholder {
          color: red;
        }
      }
      input::-webkit-outer-spin-button,
      input::-webkit-inner-spin-button {
        -webkit-appearance: none;
        margin: 0;
      }
      p {
        margin-top: -13%;
        color: red;
      }
    }
    .message {
      margin-left: 35%;
      textarea {
        padding: 6.9%;
      }
    }
  }
  button {
    cursor: pointer;
    color: white;
    font-size: 18px;
    font-weight: 600;
    display: block;
    margin: 2% auto;
    padding: 1.5% 7%;
    border: none;
    border-radius: 5px;
    line-height: 28px;
    background: rgb(255, 154, 98);
    background: linear-gradient(
      90deg,
      rgba(255, 154, 98, 1) 0%,
      rgba(255, 114, 121, 1) 50%,
      rgba(255, 68, 147, 1) 100%
    );
  }
}
</style>
