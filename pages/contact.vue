<script setup lang="ts">
import { ref } from 'vue';
import axios from 'axios';
import { useRouter } from 'vue-router';

const router = useRouter();

const name = ref('');
const email = ref('');
const phone = ref('');
const message = ref('');

const sendMail = async () => {
  try {
    const result = await axios.post('https://formspree.io/f/xrbbgqoe', {
      message: message.value,
      name: name.value,
      phone: phone.value,
      email: email.value
    });
    if (result.status === 200) {
      clearFields();
    } else {
      throw new Error('Back end problem');
    }
  } catch (err) {
    console.log(err);
  }
};

const clearFields = () => {
  name.value = '';
  email.value = '';
  phone.value = '';
  message.value = '';
};

const goBack = () => {
  router.back();
};
</script>

<template>
  <section class="contact">
		<button class="back-button" @click="goBack"><</button>
    <div class="form-container">
      <header>
        <h2 class="heading-2 bold">Demande de devis gratuit</h2>
      </header>

      <form @submit.prevent>
        <div class="form-control">
          <input placeholder="Nom et prénom" name="name" v-model="name" type="text" />
        </div>
        <div class="form-control">
          <input placeholder="Téléphone" name="phone" v-model="phone" type="tel" />
        </div>
        <div class="form-control">
          <input placeholder="Email" name="email" v-model="email" type="email" />
        </div>
        <div class="form-control">
          <textarea placeholder="Message" name="message" id="message" cols="30" rows="10" v-model="message"></textarea>
        </div>
        <div class="form-control action">
          <button class="body-text bold" @click="sendMail">Envoyer</button>
        </div>
      </form>
    </div>
  </section>
</template>

<style scoped>
.contact {
	position: relative;
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
  background-color: var(--fb-offwhite);
}

.form-container {
  background-color: var(--fb-primary);
  padding: 2rem;
  border-radius: 10px;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  width: 100%;
  max-width: 500px;
}

.back-button {
  position: absolute;
  top: 1rem;
  left: 2rem;
	width: 3.5rem;
	height: 3.5rem;
  background: none;
  border: 1px solid var(--fb-primary);
  color: var(--fb-primary);
  padding: 0.5rem 1rem;
  border-radius: 50%;
  cursor: pointer;
  font-size: 1.5rem;
}

.back-button:hover {
  background-color: var(--fb-primary);
  color: white;
}

header {
	color: var(--fb-offwhite);
  font-size: var(--fb-header-3);
	font-family: 'DM Serif Display', sans-serif;
  text-align: center;
	margin-bottom: 1.5rem;
}

.form-control {
  margin-bottom: 1rem;
}

input,
textarea {
  width: 100%;
  padding: 0.75rem;
  border: 1px solid var(--border-color);
  border-radius: 5px;
  font-size: 1rem;
  font-family: 'DM Sans', sans-serif;
}

input:focus,
textarea:focus {
  outline: none;
  border-color: var(--fb-primary);
}

button {
  width: 100%;
  padding: 0.75rem;
  background-color: var(--secondary-color);
  color: var(--fb-offwhite);
  border: 1px solid var(--fb-offwhite);
  border-radius: 5px;
  font-size: 1rem;
  cursor: pointer;
  font-family: 'DM Sans', sans-serif;
}

button:hover {
  background-color: var(--fb-offwhite);
  color: var(--fb-primary);
}

@media only screen and (max-width: 680px) { 
	.form-container {
		padding: 2rem 1rem;
		width: 90%;
	}
	.back-button {
		top: 0rem;
		
	}
}
</style>
