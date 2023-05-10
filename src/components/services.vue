<template>
    <p class="title">SERVIÇOS</p>
    <div class="column">

        <div class="row-1">
            <ServiceCard class="service-card" :title="mobileTitle" :text="mobileText" :item="mobileItem" />
            <ServiceCard class="service-card" :title="webdevTitle" :text="webdevText" :item="webdevItem" />
        </div>
            
        <div class="row-2">
            <ServiceCard class="service-card" :title="sistemasTitle" :text="sistemasText" :item="sistemasItem" />
            <ServiceCard class="service-card" :title="datascienceTitle" :text="datascienceText" :item="datascienceItem" />
        </div>

        <div class="row-3">
            <ServiceCard class="service-card" :title="educationTitle" :text="educationText" :item="educationItem" />
            <ServiceCard class="service-card" :title="consultTitle" :text="consultText" :item="consultItem" />
        </div>
    </div>
</template>

<style scoped>

.column{
    margin: 120px;
    display: flex;
    flex-direction: column;
    align-items: center;
}

.title{
    font-size: 32px;
    margin-bottom: 80px;
    margin-left: 10%;
}

.row-1{
    width: 1200px;
    display: flex;
    flex: 1;
    flex-direction: row;
}
.row-2{
    width: 1200px;
    display: flex;
    flex: 1;
    flex-direction: row;
}
.row-3{
    width: 1200px;
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
            datascienceTitle: "Business Intelligence e Ciência de Dados",
            datascienceText: "Tomar decisões baseadas em evidências é imprescindível na saúde. Utilizando tecnologias modernas para a coleta, transformação e carregamento de dados, construímos dashboards interativos para gerar informações de qualidade a partir da sua base de dados, potencializando os insights da equipe.",
            datascienceItem: "data-science.png",
            educationTitle: "Educação em Saúde",
            educationText: "Construção de artefatos digitais que sirvam de apoio à educação em saúde, buscando o desenvolvimento de soluções que possam abranger aspectos de gamificação e realidade virtual.",
            educationItem: "relatorio-de-saude.png",
            consultTitle: "Consultoria em TI",
            consultText: "O surgimento de novas tecnologias se tornou uma tendência nos últimos anos. Nossos serviços podem auxiliar no planejamento de projetos, na tomada de decisões e no acompanhamento de todas as atividades para que a sua empresa se mantenha competitiva e atuante no mercado.",
            consultItem: "consultor.png",
        }
    }
}
</script>
