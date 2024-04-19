<script setup lang="ts">
import { IP } from './store';
import SubnetStatus from './components/SubnetStatus.vue';
import SubnetForm from './components/SubnetForm.vue';
</script>

<template>
    <h1>Subnet calculator</h1>
    <SubnetForm />
    <SubnetStatus v-if="IP.isValid" />
</template>