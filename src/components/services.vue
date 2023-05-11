<template>
    <p class="title">SERVIÇOS</p>
    <div v-if="mediumScreen" class="column">
        <div class="card-row">
            <ServiceCard class="service-card" :title="mobileTitle" :text="mobileText" :item="mobileItem" />
            <ServiceCard class="service-card" :title="webdevTitle" :text="webdevText" :item="webdevItem" />
        </div>
            
        <div class="card-row">
            <ServiceCard class="service-card" :title="sistemasTitle" :text="sistemasText" :item="sistemasItem" />
            <ServiceCard class="service-card" :title="datascienceTitle" :text="datascienceText" :item="datascienceItem" />
        </div>

        <div class="card-row">
            <ServiceCard class="service-card" :title="educationTitle" :text="educationText" :item="educationItem" />
            <ServiceCard class="service-card" :title="consultTitle" :text="consultText" :item="consultItem" />
        </div>
    </div>
    <div v-if="bigScreen" class="column">
        <div class="card-row">
            <ServiceCard class="service-card" :title="mobileTitle" :text="mobileText" :item="mobileItem" />
            <ServiceCard class="service-card" :title="webdevTitle" :text="webdevText" :item="webdevItem" />
            <ServiceCard class="service-card" :title="sistemasTitle" :text="sistemasText" :item="sistemasItem" />
        </div>
        
        <div class="card-row">
            <ServiceCard class="service-card" :title="datascienceTitle" :text="datascienceText" :item="datascienceItem" />
            <ServiceCard class="service-card" :title="educationTitle" :text="educationText" :item="educationItem" />
            <ServiceCard class="service-card" :title="consultTitle" :text="consultText" :item="consultItem" />
        </div>
    </div>
</template>

<style scoped>

    @media (max-width: 1200px){
        .column{
            margin: 120px;
            display: flex;
            flex-direction: column;
            align-items: center;
        }

        .title{
            font-size: 64px;
            margin-bottom: 80px;
            margin-left: 10%;
        }

        .card-row{
            /* width: 95%; */
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
    }

    @media (max-width: 1800px) and (min-width: 1200px){
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

        .card-row{
            width: 95%;
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
    }

    
    @media (max-width:2400px) and (min-width: 1801px){
        .column{
            width: 98%;
            margin: 1%;
            display: flex;
            flex-direction: column;
            align-items: center;
        }

        .title{
            font-size: 32px;
            margin-bottom: 80px;
            margin-left: 10%;
        }

        .card-row{
            width: 100%;
            display: flex;
            flex: 1;
            flex-direction: row;
        }

        .service-card{
            /* margin-left: 5px; */
            /* margin-right: 5px; */
            
            margin-top: 15px;
            margin-bottom: 15px;
        }
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
            mediumScreen:false,
            bigScreen:false,

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
    },
    mounted() {
        window.addEventListener('resize', this.handleResize)
        this.handleResize()
    },
    methods: {
        handleResize() {
        this.mediumScreen = window.innerWidth <= 1800
        this.bigScreen = window.innerWidth > 1800
        }
    },
    beforeDestroy() {
        window.removeEventListener('resize', this.handleResize)
    }
}
</script>
