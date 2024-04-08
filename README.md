
# RespirAr

O projeto "RespirAr" visa definir um marco inovador no campo da saúde pública, com o propósito de desenvolver e implementar um sistema de monitoramento e alerta da qualidade do ar de última geração, especificamente projetado para ambientes de ensino público. 
Este sistema, dotado de sensores de última geração, tem como meta identificar de maneira precisa uma variedade de poluentes presentes no ar, oferecendo dados em tempo real através de uma interface amigável e intuitiva. O intuito é garantir que informações críticas sobre a qualidade do ar sejam facilmente acessíveis, permitindo uma resposta rápida e efetiva a qualquer momento que os níveis de poluição ultrapassem os padrões de segurança estabelecidos.


## 🚀 Começando

Essas instruções permitirão que você obtenha uma cópia do projeto em operação na sua máquina local para fins de desenvolvimento e teste.

# Nuxt 3 Minimal Starter

Look at the [Nuxt 3 documentation](https://nuxt.com/docs/getting-started/introduction) to learn more.

## Setup

Make sure to install the dependencies:

```bash
# npm
npm install

# pnpm
pnpm install

# yarn
yarn install

# bun
bun install
```

## Development Server

Start the development server on `http://localhost:3000`:

```bash
# npm
npm run dev

# pnpm
pnpm run dev

# yarn
yarn dev

# bun
bun run dev
```

## Production

Build the application for production:

```bash
# npm
npm run build

# pnpm
pnpm run build

# yarn
yarn build

# bun
bun run build
```

Locally preview production build:

```bash
# npm
npm run preview

# pnpm
pnpm run preview

# yarn
yarn preview

# bun
bun run preview
```

Check out the [deployment documentation](https://nuxt.com/docs/getting-started/deployment) for more information.

Consulte **[Implantação](#-implanta%C3%A7%C3%A3o)** para saber como implantar o projeto.

### 📋 Pré-requisitos

De que coisas você precisa para instalar o software e como instalá-lo?

```
    Node.js: Versão 18.00 ou superior. Para verificar a versão do Node.js instalada em seu sistema, execute node -v em seu terminal. Caso não tenha o Node.js instalado ou precise de uma versão mais recente, visite nodejs.org para obter instruções de instalação.

    Firmware ESP8266: Este projeto é compatível com dispositivos que utilizam o ESP8266. Garanta que seu dispositivo esteja com o firmware atualizado e pronto para ser programado com o software necessário para a comunicação com o sensor MQ135.
```

### 🔧 Instalação

Uma série de exemplos passo-a-passo que informam o que você deve executar para ter um ambiente de desenvolvimento em execução.

```

    Montagem do Sensor MQ135: Conecte o sensor MQ135 ao seu módulo ESP8266. O sensor MQ135 é utilizado para medir a qualidade do ar e detectar uma ampla gama de gases, incluindo amônia, óxido nítrico, benzeno, fumaça, e vapor de álcool.

    Conexões: Assegure-se de que as conexões entre o sensor MQ135 e o ESP8266 estejam corretas. O VCC do sensor deve ser conectado a uma fonte de 5V, o GND ao GND do ESP8266, e o sinal analógico (A0) do sensor ao pino analógico do ESP8266.

    Alimentação: Certifique-se de que o ESP8266 esteja adequadamente alimentado, seja através de USB ou com uma fonte de alimentação externa compatível.

```

## ⚙️ Executando os testes

Explicar como executar os testes automatizados para este sistema.

### 🔩 Analise os testes de ponta a ponta

Explique que eles verificam esses testes e porquê.

```
Dar exemplos
```

### ⌨️ E testes de estilo de codificação

Explique que eles verificam esses testes e porquê.

```
Dar exemplos
```

## 📦 Implantação

Adicione notas adicionais sobre como implantar isso em um sistema ativo

## 🛠️ Construído com

Para assegurar a eficiência e a qualidade no desenvolvimento do front-end e do back-end, será adotado o Git, um sistema de controle de versões distribuído. O Git é essencial para o gerenciamento eficaz das alterações no código, possibilitando a colaboração em equipe, facilitando o rastreamento de cada modificação e coordenando tarefas entre os desenvolvedores. Além do uso do Git, serão incorporados princípios de metodologias ágeis, incluindo:

Scrum: Foca na gestão e planejamento de projetos em sprints, períodos curtos de tempo durante os quais tarefas específicas devem ser completadas. O Scrum é adaptável a projetos complexos, promovendo a entrega contínua de valor por meio de revisões regulares e adaptações do plano de projeto.

Kanban: Visa a otimização dos fluxos de trabalho. Caracteriza-se pelo uso de quadros visuais para representar as tarefas, permitindo uma visão clara do progresso e facilitando a identificação de gargalos no desenvolvimento.

Programação em Par (Pair Programming): Uma prática onde dois programadores trabalham juntos em um único computador, um escrevendo o código enquanto o outro revisa cada linha conforme é digitada. Esta colaboração melhora a qualidade do código e a disseminação do conhecimento entre a equipe.

Integração Contínua (CI) e Entrega Contínua (CD): Práticas de engenharia de software que visam à automação das fases de teste e entrega. Garantem que cada alteração no código seja automaticamente testada e pronta para produção, agilizando o ciclo de vida do desenvolvimento de software.

A adoção dessas metodologias e práticas visa não apenas agilizar o desenvolvimento do projeto, mas também assegurar que o produto final seja robusto, confiável e capaz de satisfazer as necessidades dos usuários finais de forma eficiente.


Desenvolvimento do Frontend


Para a construção da interface do usuário neste projeto, optou-se por um conjunto de ferramentas e tecnologias de ponta que garantem tanto a eficiência do desenvolvimento quanto a qualidade do produto final. Os recursos selecionados são:

Visual Studio Code: Este editor de código fonte, criado pela Microsoft, é compatível com Windows, Linux e macOS. Reconhecido por sua versatilidade, o Visual Studio Code oferece funcionalidades como depuração integrada, controle de versionamento Git, realce de sintaxe, autocompletar inteligente, snippets e ferramentas de refatoração de código, facilitando significativamente o processo de desenvolvimento.

HTML (Hypertext Markup Language): A base para a construção de websites, o HTML permite a estruturação de páginas web e a incorporação de conteúdo multimídia, como imagens e vídeos, através de hipertextos. Sua utilização é fundamental para definir a estrutura básica da plataforma.

CSS (Cascading Style Sheets): CSS é a linguagem de estilo que, quando usada em conjunto com HTML, permite a personalização visual das páginas, incluindo layout, cores e fontes, essencial para a criação de uma experiência de usuário atrativa e coesa.

JavaScript: Uma linguagem de programação poderosa que adiciona interatividade às páginas web, permitindo a implementação de funcionalidades complexas e melhorando significativamente a experiência do usuário.

Vue.js: Uma biblioteca JavaScript progressiva para construir interfaces de usuário. Vue.js é desenhado para ser adaptável, podendo ser integrado a projetos já existentes ou utilizado em complexos sistemas de Single Page Applications quando usado em conjunto com ferramentas modernas e bibliotecas de apoio.

React Native: Esta tecnologia permite o desenvolvimento de aplicativos móveis nativos para iOS e Android usando JavaScript, facilitando a criação de experiências de usuário ricas e performáticas em dispositivos móveis, com um único código-base.

Nuxt.js: Este framework baseado em Vue.js facilita a criação de aplicações universais, seja para Single Page Applications, aplicações renderizadas pelo servidor ou sites estáticos. Ele se destaca ao otimizar a experiência do usuário e melhorar o desempenho, reduzindo significativamente os tempos de carregamento das páginas, além de oferecer uma configuração simplificada que acelera o desenvolvimento de projetos web.


PrimeVue: Uma biblioteca rica em componentes de interface do usuário para Vue.js, que acompanha um sistema de temas personalizáveis através do Theme Designer, permitindo a criação de interfaces atrativas e coesas com facilidade.

PrimeFlex: Uma biblioteca de utilitários CSS que facilita a criação de layouts responsivos e flexíveis, permitindo um design adaptativo e fluido que responde a diferentes tamanhos de tela e dispositivos.


Componentes Utilizados


ESP8266: Este módulo Wi-Fi foi escolhido por sua capacidade de conectar o sistema à internet sem a necessidade de componentes adicionais. Ele permite o envio de dados em tempo real para o backend, facilitando o monitoramento remoto.

Sensor MQ135: Utilizado para a detecção de gases nocivos e a qualidade geral do ar. Este sensor é capaz de detectar uma ampla gama de gases, incluindo amônia, óxidos de nitrogênio, benzeno, fumaça e dióxido de carbono.

Sensor DHT11: Fornece leituras de temperatura e umidade, componentes cruciais para avaliar a qualidade do ar interior.

Display LCD : Exibe localmente as leituras dos sensores, incluindo qualidade do ar, temperatura e umidade, permitindo uma visualização rápida e fácil pelos responsáveis pela manutenção dos ambientes monitorados.

Cabos de Conexão: Utilizados para interligar os componentes eletrônicos e o módulo ESP8266.

Desenvolvimento do Backend

O sistema "RespirAr" adota uma arquitetura cliente-servidor sofisticada, onde o componente backend assume uma função essencial no processamento e armazenagem de dados relacionados à qualidade do ar, os quais são coletados em tempo real. Para o desenvolvimento deste backend, optou-se pela utilização de Java, reconhecida por sua robustez, segurança e versatilidade, o que a torna uma escolha ideal para a construção de sistemas confiáveis e de alta performance. O gerenciamento dos dados coletados é realizado através de um banco de dados MySQL, selecionado devido à sua excelente capacidade de escalabilidade, confiabilidade e suporte efetivo para um alto volume de transações.

A transferência de dados dos sensores até o servidor é efetuada por meio de requisições Rest API, uma estratégia que promove uma integração segura e eficiente entre o hardware e o backend. A fim de garantir uma comunicação segura e confiável, o sistema emprega mecanismos de autenticação e criptografia para proteger as transmissões de dados.

Uma vez no servidor, os dados passam por um processamento criterioso: são validados, organizados e então persistidos no banco de dados MySQL. Este procedimento não apenas facilita a recuperação e análise futuras dos dados, mas também permite uma gestão eficaz e um monitoramento em tempo real da qualidade do ar. Ademais, a plataforma é dotada de um sistema de alertas personalizáveis, que são configurados para notificar os usuários finais em casos de detecção de valores que excedam os limites pré-estabelecidos para variáveis ambientais como a qualidade do ar, temperatura e umidade. Esses alertas são fundamentais para a tomada de decisões rápidas e informadas em ambientes críticos como escolas e hospitais.

Para maximizar a eficiência e segurança do projeto, foram implementadas práticas e metodologias de desenvolvimento modernas, incluindo a utilização de Git para o controle de versões, o que facilita a colaboração entre os desenvolvedores e assegura um registro detalhado de todas as modificações feitas no código. Além disso, o emprego de técnicas de desenvolvimento ágil e revisões constantes de código visa aprimorar a qualidade e a confiabilidade do software.
Essa abordagem integral ao desenvolvimento e manutenção do backend do "RespirAr" permite que o sistema não apenas funcione efetivamente, coletando e analisando dados sobre a qualidade do ar em tempo real, mas também seja escalável, seguro e adaptável às necessidades futuras, oferecendo assim uma solução duradoura e flexível para o monitoramento ambiental em instituições vitais como escolas e hospitais.

## ✒️ Autores

Mencione todos aqueles que ajudaram a levantar o projeto desde o seu início

* **Maicon Douglas Mendes Alves** - *Trabalho Inicial* - [umdesenvolvedor](https://github.com/linkParaPerfil)
* **Carlos Alberto de Aguiar** - *Trabalho Inicial* - [umdesenvolvedor](https://github.com/linkParaPerfil)
* **João Marcos Racanelli** - *Trabalho Inicial* - [umdesenvolvedor](https://github.com/linkParaPerfil)
* **Leonardo Marcondeli** - *Trabalho Inicial* - [umdesenvolvedor](https://github.com/linkParaPerfil)
* **Vinicius de Moraes de Godoi** - *Trabalho Inicial* - [umdesenvolvedor](https://github.com/linkParaPerfil)

## 📄 Licença

Este projeto está sob a licença (sua licença) - veja o arquivo [LICENSE.md](https://github.com/usuario/projeto/licenca) para detalhes.