<template>
    <div class="container-fluid">
        <index/>
        <Languajes/>
    </div>
</template>
<script>
    import { defineComponent } from 'vue';
    import Index from '../components/home/index.vue'
    import Languajes from '../components/home/languajes.vue'
    export default defineComponent({
        name: 'Home',
        components: {
            Index,
            Languajes
        },
        data() {
            return {
            }
        },
        methods: {
        }
    });
</script>
