<template>
    <div class="mx-auto w-75">
        <div class="title m-b-md">
            <h1>Welcome to my portfolio</h1>
        </div>
        <div class="links">
            <router-link v-bind:to="{name: 'top'}">
                <button class="btn btn-outline-dark btn-lg">top</button>
            </router-link>
            <router-link v-bind:to="{name: 'about'}">
                <button class="btn btn-outline-dark btn-lg">about this page</button>
            </router-link>
            <router-link v-bind:to="{name: 'skills'}">
                <button class="btn btn-outline-dark btn-lg">skills</button>
            </router-link>
            <router-link v-bind:to="{name: 'introduction'}">
                <button class="btn btn-outline-dark btn-lg">introduction</button>
            </router-link>
        </div>
    </div>
</template>