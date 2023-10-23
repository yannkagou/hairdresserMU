<template>
    <main>
        <div class="modal-body">
            <div class="title">Make an appointment</div>

            <form class="profile-form" @submit.prevent="saveAppointmentForm">

                <div class="form-items">
                    <div class="form-group">
                        <label class="input-label">Your Name</label>
                        <input class="email" v-model="appointmentform.name" type="text" id="appointmentname"
                            placeholder="Name..." required>
                    </div>
                    <div class="form-group">
                        <label class="input-label">Your Email</label>
                        <input class="email" v-model="appointmentform.email" type="email" id="appointmentemail"
                            placeholder="Email..." required>
                    </div>
                </div>

                <div class="form-items">
                    <div class="form-group">
                        <label class="input-label">Service Needed</label>
                        <input class="email" v-model="appointmentform.service" type="text" id="appointmentservice"
                            placeholder="Service you need..." required>
                    </div>
                    <div class="form-group">
                        <label class="input-label">Date</label>
                        <input class="email" v-model="appointmentform.date" type="date" id="appointmentdate"
                            placeholder="Date..." required>
                    </div>
                </div>

                <div class="form-items2">
                    <label class="input-label">Your Message</label>
                    <textarea class="email" v-model="appointmentform.message"  id="appointmentmessage" rows="4"
                        cols="50" placeholder="Enter your message..." required></textarea>
                </div>

                <div class="footer2">
                    <button class="cancel" @click="cancelAppointment">Cancel</button>
                    <div class="footer-left">
                        <button @click="saveAppointmentForm" class="submit" type="submit">Send</button>
                    </div>
                </div>

            </form>

        </div>

        
    </main>
</template>

<script setup>
import { ref, reactive } from 'vue';

let appointmentform = reactive({
    name: '',
    email: '',
    service: '',
    date: '',
    message: '',
})

const cancelAppointment = () => {
    appointmentform.name = '';
    appointmentform.email = '';
    appointmentform.service = '';
    appointmentform.date = '';
    appointmentform.message = '';
}

function saveAppointmentForm() {
    console.log(appointmentform.value)
}
</script>