<template>
    <navbar></navbar>

    <router-view></router-view>

    <!-- <page-viewer :page="pages[activePage]"></page-viewer> -->

    <!-- <create-page @page-created="pageCreated"></create-page> -->
</template>

<script>
import Navbar from './components/Navbar.vue';

export default {
    components: {
        Navbar,
    },
    methods: {
        pageCreated(pageObj) {
            this.pages.push(pageObj);
        }
    },
}
</script>