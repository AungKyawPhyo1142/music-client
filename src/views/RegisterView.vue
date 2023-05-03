<template>
    <div id="Register">
        <div class="w-full p-6 flex justify-center items-center">
            <div class="w-full max-w-xs">

            <div class="bg-black p-8 shadow rounded mb-6">
                <h1 class="mb-6 text-lg text-gray-100 font-thin">
                    Let's get Rocking
                </h1>
                <div class="mb-4">
                    <TextInput
                    label="First Name"
                    :labelColor=false
                    placeholder="John"
                    v-model:input="firstName"
                    inputType="text"
                    error="This is"
                    />
                    
                </div>
                <div class="mb-4">
                    <TextInput
                    label="Last Name"
                    :labelColor=false
                    placeholder="Doe"
                    v-model:input="lastName"
                    inputType="text"
                    error="This is a test error"
                    />
                    
                </div>
                <div class="mb-4">
                    <TextInput
                    label="Email"
                    :labelColor=false
                    placeholder="john.doe@gmail.com"
                    v-model:input="email"
                    inputType="text"
                    error="This is a test error"
                    />
                </div>
                <div class="mb-4">
                    <TextInput
                    label="Password"
                    :labelColor=false
                    placeholder="password123"
                    v-model:input="password"
                    inputType="password"
                    error="This is a test error"
                    />
                    
                </div>
                <div class="mb-4">
                    <TextInput
                    label="Confirm Password"
                    :labelColor=false
                    placeholder="password123"
                    v-model:input="confirmPassword"
                    inputType="password"
                    error="This is a test error"
                    />

                </div>
                <button 
                    class="
                    block
                    w-full
                    bg-green-500
                    text-white
                    rounded-sm
                    py-3
                    text-sm
                    tracking-wide
                    "
                    type="submit"
                    >
                Register
                </button>
            </div>
            <p class="text-center text-md text-gray-500">
                Already have an account?
                <router-link to="login" class="text-blue-500 no-underline hover:underlink">
                    Login
                </router-link>
            </p>
        </div>

        </div>
    </div>
</template>

<script setup>
import { ref } from "vue";
import TextInput from "../components/global/TextInput.vue"

let firstName = ref(null)
let lastName = ref(null)
let email = ref(null)
let password = ref(null)
let confirmPassword = ref(null)
</script>

<style lang="scss">

</style>
