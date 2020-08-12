<template>
    <div class="container-fluid bg-dark mb-3">
        <div class="container">
            <nav class="navbar navbar-dark">
                <span class="navbar-brand mb-0 h1">Vue と Laravel で SPA</span>
                <div>
                    <router-link v-bind:to="{name: 'top'}">
                        <button class="btn btn-outline-light btn-sm">top</button>
                    </router-link>
                    <router-link v-bind:to="{name: 'about'}">
                        <button class="btn btn-outline-light btn-sm">about this page</button>
                    </router-link>
                    <router-link v-bind:to="{name: 'skills'}">
                        <button class="btn btn-outline-light btn-sm">skills</button>
                    </router-link>
                    <router-link v-bind:to="{name: 'introduction'}">
                        <button class="btn btn-outline-light btn-sm">introduction</button>
                    </router-link>
                </div>
            </nav>
        </div>
    </div>
</template>

<script>
    export default {}
</script>