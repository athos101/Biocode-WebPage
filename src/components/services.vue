<template>
    <div class="column">
        <p class="title">SERVIÇOS</p>

        <div class="row-1">
            <ServiceCard class="service-card" :title="mobileTitle" :text="mobileText" :item="mobileItem" />
            <ServiceCard class="service-card" :title="webdevTitle" :text="webdevText" :item="webdevItem" />
        </div>

        <div class="row-2">

        </div>

        <div class="row-3">

        </div>
    </div>
</template>

<style scoped>

.column{
    margin: 120px;
    display: flex;
    flex-direction: column;
}

.title{
    font-size: 32px;
    margin-bottom: 80px;
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
    /* margin-left: 5px; */
    /* margin-right: 5px; */
    margin-top: 10px;
    margin-bottom: 10px;
}

</style>

<script>
import ServiceCard from './service-card.vue'

export default {
    name: 'Services',
    components:{
        ServiceCard,
    },
    data(){
        return{
            mobileTitle: "Desenvolvimento Mobile",
            mobileText: 'A praticidade dos dispositivos móveis e a internet diminuem a distância entre pessoas e serviços. Por isso, desenvolvemos aplicativos que sirvam de ferramenta para o trabalho em saúde, comunicação, automatização de processos, registro e muito mais.',
            mobileItem: "smartphone.png",
            webdevTitle: "Desenvolvimento Web",
            webdevText: "O mundo está na web. Conecte o seu negócio ou perfil com o restante do mundo por meio de websites interativos e responsivos. Nós também podemos oferecer APIs totalmente personalizadas às suas necessidades.",
            webdevItem: "computador.png",
            sistemasTitle: "Sistemas de Informação",
            sistemasText: "Podemos te ajudar a manter seus dados mais organizados e seguros por meio de sistemas personalizados de acordo com as suas necessidades, podendo estes serem integrados aos sistemas já existentes.",
            sistemasItem: "sistema-operacional.png",
        }
    }
}
</script>
