<template>
    <div class="container-fluid">
        <Contact/>
    </div>
</template>
<script>
    import { defineComponent } from 'vue';
    import Contact from '../components/about/contact.vue'
    export default defineComponent({
        name: 'About',
        components: {
            Contact
        },
    });
</script>
