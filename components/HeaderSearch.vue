<script setup>
const carReg = useCarRegistrationrStore();

</script>

<template>
    <input type="text" id="base-input" placeholder="Enter Reg" v-model="carReg.reg_number"
        @input="carReg.reg_number = $event.target.value.toUpperCase()" @keyup.enter="carReg.submitCarRegistrationNumber"
        class="bg-gray-50 border border-gray-300 
            text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full p-2.5 
            dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-blue-500 
            dark:focus:border-blue-500" />
</template>