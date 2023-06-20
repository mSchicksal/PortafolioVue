<template>
    <div class="container-fluid">
        <div class="row app-navbar app-flex-center">
            <div class="col-1 app-flex-start">
                <i class="bi bi-code-square"/>
                &nbsp;
                <RouterLink to="/">Álvaro C.</RouterLink>
            </div>
            <div class="col-10 app-flex-center">
                <a href="https://www.linkedin.com/in/alvaro-catal%C3%A1n-zavala-b6238b1a2/">
                    <i class="bi bi-linkedin"/>
                </a>
                &nbsp;
                <a href="https://github.com/mSchicksal">
                    <i class="bi bi-github"/>
                </a>

            </div>
            <div class="col-1 app-flex-end">
                <!-- <i v-if="theme" @click="setTheme" class="bi bi-brightness-high"/>
                <i v-else @click="setTheme" class="bi bi-moon"/> -->
                <i class="bi bi-chat"/>
                &nbsp;
                <RouterLink to="/about">Hire Me</RouterLink>
            </div>
        </div>
        <div class="row app-body">
            <RouterView />
        </div>
    </div>
</template>
<script>
    import { defineComponent } from 'vue';
    import { RouterLink, RouterView } from 'vue-router'
    export default defineComponent({
        name: 'App',
        components: {},
        data() {
            return {
                theme: true,
            }
        },
        methods: {
            setTheme() {
                let t = this;
                t.theme = t.theme == false ? true: false;
                if(t.theme == false) {
                    this.root.style.setProperty("--first-color", "#8892B0");
                    this.root.style.setProperty("--second-color", "#4BBEA9");
                    this.root.style.setProperty("--third-color", "#0A192F");
                    this.root.style.setProperty("--fourth-color", "#0A192F");
                } else {
                    this.root.style.setProperty("--first-color", "#8892B0");
                    this.root.style.setProperty("--second-color", "#4BBEA9");
                    this.root.style.setProperty("--third-color", "#0A192F");
                    this.root.style.setProperty("--fourth-color", "#ffffff");
                }
            },
        }
    });
</script>
<style>
    @import './assets/css/App.css';
    @import './assets/css/Navbar.css';
</style>
