<template>
    <div class="column">
        <div class="row-1">
            <div class="service-card"><ServiceCard /></div>
            <div class="service-card"><ServiceCard /></div>
        </div>
        <div class="row-2">
            <div class="service-card"><ServiceCard /></div>
            <div class="service-card"><ServiceCard /></div>
        </div>
        <div class="row-3">
            <div class="service-card"><ServiceCard /></div>
            <div class="service-card"><ServiceCard /></div>
        </div>
    </div>
</template>

<style scoped>

.column{
    margin: 5%;
    display: flex;
    flex-direction: column;
}

.row-1{
    display: flex;
    flex: 1;
    flex-direction: row;
}
.row-2{
    display: flex;
    flex: 1;
    flex-direction: row;
}
.row-3{
    display: flex;
    flex: 1;
    flex-direction: row;
}

.service-card{
    margin: 15px;
}

</style>

<script>
import ServiceCard from './service_card.vue'

export default {
    components:{
        ServiceCard,
    }
}
</script>
