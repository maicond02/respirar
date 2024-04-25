<template>
    <section>
        <div>
            <section class="grid">
                <div class="col-12 md:col-6 mt-8">
                    <div class="flex flex-column align-items-center">
                        <span class="text-xl md:text-6xl font-semibold">Bem-vindo ao <strong class="text-blue-500">RespirAr</strong>:</span>
                        <span class="text-xl md:text-6xl font-semibold">Monitoramento Avançado de Qualidade do Ar</span>
                    </div>
                    <div>
                        <p>O projeto "RespirAr" surge como uma iniciativa inovadora no campo da saúde pública e tecnologia ambiental, mirando o desenvolvimento e a implementação de um sistema avançado de monitoramento e alerta da qualidade do ar, especialmente para ambientes de ensino público. Este sistema promete transformar o ambiente educacional, tornando-o mais saudável e seguro para estudantes e professores. Com a utilização de tecnologias de ponta, o projeto visa detectar uma ampla gama de poluentes - como dióxido de carbono, amônia e partículas alergênicas - fornecendo dados em tempo real essenciais para a tomada de decisões e a manutenção de um ar puro nas salas de aula. Central para o "RespirAr" é o desenvolvimento de um hardware robusto e uma plataforma digital interativa, que oferece não apenas a coleta de dados, mas também sua análise detalhada através de um software intuitivo. Essa interface amigável é projetada para ser facilmente manejável por administradores escolares, permitindo-lhes monitorar a qualidade do ar continuamente e com precisão.</p>
                    </div>
                    <div class="w-12 flex justify-content-center">
                        <Button label="Conheça nosso sistema" class="w-4 text-white" />
                    </div>
                </div>
                <div class="col-12 md:col-6">
                    <img src="@/assets/images/college.png" alt="college" width="100%">
                </div>
                <div class="grid equal-height">
                    <div class="col-12 md:col-4">
                        <div class="shadow-2 bg-card p-2 text-black-alpha-90">
                            <p class="">O <strong>RespirAr</strong> é o mais novo sistema de monitoramento da qualidade do ar, projetado para fornecer dados precisos e em tempo real sobre a qualidade do ar em sua comunidade. Com a tecnologia de ponta e sensores avançados, nosso sistema identifica uma ampla gama de poluentes, garantindo que você e sua família respirem um ar mais limpo e seguro.</p>
                        </div>
                    </div>
                    <div class="col-12 md:col-4">
                        <div class="shadow-2 bg-card p-2 text-black-alpha-90">
                            <h2>Por que escolher o RespirAr?</h2>
                            <ul>
                                <li><strong>Dados Precisos em Tempo Real:</strong> Nosso sistema utiliza a mais recente tecnologia de sensores para fornecer atualizações instantâneas sobre a qualidade do ar.</li>
                                <li><strong>Fácil de Usar:</strong> A interface do usuário do RespirAr é intuitiva, tornando fácil para todos monitorarem a qualidade do ar em suas áreas.</li>
                                <li><strong>Impacto Positivo na Saúde:</strong> Com informações detalhadas sobre a qualidade do ar, você pode tomar medidas proativas para proteger sua saúde e bem-estar.</li>
                            </ul>
                        </div>
                    </div>
                    <div class="col-12 md:col-4">
                        <div class="shadow-2 bg-card p-2 text-black-alpha-90">
                            <h3>Entre em Contato</h3>
                            <p>Interessado em saber mais sobre o RespirAr e como ele pode beneficiar você ou sua comunidade? Entre em contato conosco através de nosso <a href="url_para_contato">formulário de contato</a> para mais informações.</p>
                        </div>
                    </div>
                </div>
            </section>
        </div>
    </section>
</template>

<style scoped>
    .bg-card{
        background-color: #60a5fa;
        border-radius: 4px;
        color: white !important;
    }
    a{
        color: white;
    }
    .equal-height {
        display: flex;
    }
  
  .equal-height .col-12 {
    display: flex;
    flex-direction: column;
  }
  
  .equal-height .col-12 .shadow-2 {
    flex: 1;
  }
</style>