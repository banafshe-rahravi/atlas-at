<template>
    <ul class="cards">
        <slot />
    </ul>
</template>
<script setup>


</script>
<style scoped>
.cards {
    display: inline-block;
    padding-left: 78px;
}

.card-content {
    font-family: Inter;
    font-size: 14px;
    font-weight: 400;
    line-height: 20px;
    letter-spacing: 0em;
    text-align: left;
    margin-bottom: 100px;
}
</style>