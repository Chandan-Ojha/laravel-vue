<template></template>

<script>
import useCompanies from "../../composables/companies.js";
import { onMounted } from "vue";

export default {
    setup() {
        const { companies, getCompanies } = useCompanies();
        onMounted(getCompanies);
        return { companies, getCompanies };
    },
};
</script>
