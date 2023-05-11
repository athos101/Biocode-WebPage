<template>
    <div class = "fundo">
        <div class="colum"> 
            <div class="row"> 
                <div class="historia">
                    <h1>História</h1>
                    <p>Nascemos da vontade de preencher uma área ainda pouco explorada no mercado de trabalho, 
                    mas com um potencial enorme nos próximos anos. Aspiramos tornar estudantes em profissionais 
                    qualificados nas áreas interdisciplinares trabalhadas durante a graduação de Informática 
                    Biomédica, como a Biotecnologia, Bioinformática e Telessaúde.</p>
                </div>
                <div class="circulo">
                    <img class="image" src="../assets/img-hist.png">
                </div>
            </div> 
                <div class="row">
                    <div class="missao">
                        <h1 style="color:#0A1D3E">Missão</h1> 
                        <p style="color:#0A1D3E">Oferecer soluções na área de informática em saúde e bioinformática personalizadas, 
                        de excelência, promovendo o desenvolvimento pessoal, acadêmico e profissional de nossos membros.</p>
                    </div> 
                    <div style="width:35px">
                    <img class="image2" src="../assets/img-missao.png">
                    </div>
                    <div class="visao">
                        <h1>Visão</h1> 
                        <p>Ser uma empresa reconhecida, que atinja todo seu potencial, e sirva de referência como 
                        prestadora de serviços na sua total área de atuação em âmbito nacional e internacional.</p>
                    </div> 
                </div>
            </div>
    </div>
</template>

<script>
    export default {
        name: "Historia",
    };
</script>

<style scoped>
    .fundo{
        padding:30px;
        margin: 120px;        
        flex-direction: column;
        background: rgba(217, 217, 217, 0.1);
        border-radius: 30px;
        display:flex;
    }

    .historia{
        height:50%;
        width:70%;   
        padding-bottom:10px;
    }

    .image{
        height:250px;
        align:center;
        position:absolute;
        right:5%;
    }

    .image2{
        height: 250px;
        allign:center;
        position: absolute;
        right:43%;
    }

    .circulo{
        position:absolute;
        right:15%;
        width:170px;
        height:170px;
        border-radius:50%;
        background-color:#F84D80;
    }

    .column{
        vertical-align:top;
    }

    .row{
        display: flex;
        align-items: start;
        justify-content:space-between;
    }

    .missao{
        padding-left:30px;
        padding-right:50px;
        width:40%;
        background:#49A4EF;
        border-radius: 30px;
        color: #0A1D3E;
    }

    .visao{
        width:40%;
        height:50%;
        background:#114882;
        border-radius: 30px;
        padding-left:30px;
    }
    
    h1{
       color:white;
       font-family: Montserrat;
    }

</style>