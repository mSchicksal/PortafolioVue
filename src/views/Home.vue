<template>
    <div class="container-fluid" style="padding: 0">
        <index/>
        <Languajes/>
        <Footer/>
    </div>
</template>
<script>
    import { defineComponent } from 'vue';
    import Index from '../components/home/index.vue'
    import Languajes from '../components/home/languajes.vue'
    import Footer from '../components/home/footer.vue'
    export default defineComponent({
        name: 'Home',
        components: {
            Index,
            Languajes,
            Footer,
        },
    });
</script>
