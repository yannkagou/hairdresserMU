<template>
    <div class="popup-form">
        <div class="popup-form-content">

            <button class="close-button" @click="cancelAppointmentForm">
                <i class="fa-solid fa-x"></i>
            </button>
            <div class="modal-body">
                <div class="title">Make an appointment</div>

                <form class="profile-form" @submit.prevent="saveAppointmentForm">

                    <div class="form-items">
                        <div class="form-group">
                            <label class="input-label">Your Name</label>
                            <input class="email" type="text" id="appointmentname" v-model="appointmentform.name"
                                placeholder="Name..." required>
                        </div>
                        <div class="form-group">
                            <label class="input-label">Your Email</label>
                            <input class="email" type="email" id="appointmentemail" v-model="appointmentform.email"
                                placeholder="Email..." required>
                        </div>
                    </div>

                    <div class="form-items">
                        <div class="form-group">
                            <label class="input-label">Service Needed</label>
                            <input class="email" type="text" id="appointmentservice" v-model="appointmentform.service"
                                placeholder="Service you need..." required>
                        </div>
                        <div class="form-group">
                            <label class="input-label">Date</label>
                            <input class="email" type="date" id="appointmentdate" v-model="appointmentform.date"
                                placeholder="Date..." required>
                        </div>
                    </div>

                    <div class="form-items2">
                        <label class="input-label">Your Message</label>
                        <textarea class="email" v-model="appointmentform.message" id="appointmentmessage" rows="4"
                            cols="50" placeholder="Enter your message..." required></textarea>
                    </div>

                    <div class="footer2">
                        <button class="cancel" @click="cancelAppointmentForm">Cancel</button>
                        <div class="footer-left">
                            <button @click="saveAppointmentForm" class="submit" type="submit">Send</button>
                        </div>
                    </div>

                </form>

            </div>

        </div>
    </div>
</template>

<script setup>
import { ref, reactive } from 'vue';

defineProps({
    showAppointment: Boolean,
});
const emits = defineEmits(['showAppointmentPopup']);

const cancelAppointmentForm = () => {
    emits('showAppointmentPopup');
}
let appointmentData = ref([])

// let showAppointment = ref(false)

let appointmentform = reactive({
    name: '',
    email: '',
    service: '',
    date: '',
    message: '',
})


// function showAppointmentPopup() {
//     showAppointment.value = !showAppointment.value
// }

function saveAppointmentForm() {
    appointmentData.value.push(appointmentform)
    console.log(appointmentData.value)
}
</script>

<style>
.popup-form {
  position: fixed;
  overflow-y: scroll;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  width: 100%;
  /* height: 100%; */
  background-color: rgba(0, 0, 0, 0.5);
  padding: 20px;
  z-index: 9999;
  display: flex;
  justify-content: center;
  align-items: center;
}
.popup-form-content {
  width: 75%;
  margin: auto;
  background-color: #fff;
  border-radius: 8px;
  padding: 0px 16px;
  box-shadow: 0 2px 8px rgba(0, 0, 0, 0.15);
  position: relative;
}
.popup-form-content .close-button {
  display: block;
  position: absolute;
  width: 48px;
  height: 48px;
  border-radius: 50%;
  border: none;
  background: rgb(255, 255, 255);
  box-shadow: rgba(39, 40, 51, 0.16) 0px 8px 16px;
  top: -16px;
  right: -16px;
  outline: var(--primary);
}

.modal-body {
  display: flex;
  flex-direction: column;
}
.modal-body .title {
  font-size: 20px;
  font-weight: bold;
  display: flex;
  justify-content: center;
  align-items: center;
  color: rgba(0, 0, 0, 0.85);
  border-bottom: 1px solid #eee;
  margin-bottom: 40px;
  padding-top: 5px;
}

.modal-body .profile-form {
  margin-top: 25px;
  display: flex;
  flex-direction: column;
  width: 95%;
  margin: 0 auto;
  min-height: 0;
  text-align: left;
  padding: 0;
  color: #000;
  font-size: 14px;
  line-height: 1.5715;
  list-style: none;
  box-shadow: none;
}
.modal-body .profile-form .form-items {
  display: flex;
  align-items: center;
  justify-content: space-between;
  margin-bottom: 20px;
}
.modal-body .profile-form .form-items .form-group {
  width: 48%;
  display: flex;
  flex-direction: column;
}
.input-label {
  padding-bottom: 5px;
  color: rgba(0, 0, 0, 0.85);
  font-size: 12px;
  margin-bottom: 5px;
}
.input-label::after {
  display: inline-block;
  margin-right: 4px;
  margin-left: 2px;
  color: #ff4d4f;
  font-size: 14px;
  line-height: 1;
  content: "*";
}
.email {
  line-height: 1;
  padding: 8px;
  border-radius: 14px;
  border: 1px solid #ccc;
}
.email:hover {
  border-color: var(--primary-hover);
  border-right-width: 1px !important;
}
textarea:hover {
  border-color: var(--primary-hover) !important;
}

.email:focus {
  border-color: var(--primary-hover);
  box-shadow: 0 0 0 2px var(--primary-hover);
  border-right-width: 1px !important;
  outline: 0;
}

.modal-body .profile-form .form-items2 {
  display: flex;
  flex-direction: column;
  margin-bottom: 30px;
}
.modal-body .profile-form .form-items2 input {
  width: 100%;
}

.cancel {
  line-height: 1;
  display: inline-block;
  font-weight: 400;
  text-align: center;
  cursor: pointer;
  transition: all 0.3s cubic-bezier(0.645, 0.045, 0.355, 1);
  height: 30px;
  padding: 8px 15px;
  font-size: 12px;
  border-radius: 12px;
  background: #fff;
  min-width: 20px;
  border: 1px solid var(--primary);
  color: var(--primary);
  margin-right: 5px;
  outline: 0;
}
.submit {
  line-height: 1;
  display: inline-block;
  font-weight: 400;
  text-align: center;
  cursor: pointer;
  transition: all 0.3s cubic-bezier(0.645, 0.045, 0.355, 1);
  height: 30px;
  padding: 8px 15px;
  font-size: 12px;
  border-radius: 12px;
  background: var(--primary);
  min-width: 20px;
  border: 1px solid var(--primary);
  color: #fff;
  outline: 0;
}
.cancel:focus {
  outline: 0;
}
.submit:focus {
  outline: 0;
}

.footer2 {
  display: flex;
  align-items: center;
  justify-content: space-between;
  margin-bottom: 20px;
}
</style>