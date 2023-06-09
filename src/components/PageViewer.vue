<template>
    <div class="container">
        <h1 class="emphasize">title: {{ page.pageTitle }}</h1>
        <p>content: {{ page.content }}</p>
    </div>
</template>

<script>
export default {
    props: {
        page: {
            type: Object,
            default(rawProps) {
                return {
                    pageTitle: '',
                    content: ''
                }
            }
        }
    }
}
</script>

<style scoped>
.emphasize {
    color: blue;
}
</style>