<template>
    <div>
       <UForm @submit="processForm">
        <UFormField label="First Name">
            <UInput v-model="firstName"></UInput>
        </UFormField>
        <UFormField label="Last Name">
            <UInput v-model="lastName"></UInput>
        </UFormField>
        <UButton type="submit">
            Submit
        </UButton>
       </UForm>
       <div v-if="submitted == true">
        Hi, my first name is {{ submittedFirstName }} {{ submittedLastName }}
       </div>
    </div>
</template>
<script setup>
const firstName = ref('')
const submittedFirstName = ref('')
const lastName = ref('')
const submittedLastName = ref('')
const submitted = ref(false)
function processForm(event){
    submitted.value = true;
    submittedFirstName.value = firstName.value;
    firstName.value = '';
    submittedLastName.value = lastName.value;
    lastName.value = '';
    alert(`Hi ${submittedFirstName.value} ${submittedLastName.value}`)
}
</script>