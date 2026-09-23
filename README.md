<div align="center">

<img width="100%" alt="" src="https://capsule-render.vercel.app/api?type=waving&color=0:1A1B27,55:414868,100:70A5FD&height=200&section=header&text=Eliel%20Mesquita&fontSize=50&fontColor=FFFFFF&fontAlignY=34&desc=Desenvolvedor%20Back-End%20%20%7C%20%20Java%20%C2%B7%20Spring%20Boot%20%C2%B7%20Python&descAlignY=55&descSize=16" />

<a href="./README.md"><img alt="Português" src="https://img.shields.io/badge/Portugu%C3%AAs-70A5FD?style=flat-square&labelColor=1A1B27" /></a>
<a href="./README_EN.md"><img alt="English" src="https://img.shields.io/badge/English-24283B?style=flat-square&labelColor=1A1B27" /></a>

[![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=21&pause=1200&color=70A5FD&center=true&vCenter=true&width=560&height=45&lines=APIs+REST+em+Java+e+Spring+Boot;Arquitetura+em+camadas+e+microsservi%C3%A7os;Do+suporte+t%C3%A9cnico+para+o+back-end)](https://github.com/eliel2107)

<a href="https://www.linkedin.com/in/eliel-mesquita0799/"><img alt="LinkedIn" src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" /></a>
<a href="mailto:eliel.mesquita@gmail.com"><img alt="Gmail" src="https://img.shields.io/badge/Gmail-EA4335?style=for-the-badge&logo=gmail&logoColor=white" /></a>

</div>

## Sobre mim

Desenvolvedor **Back-End**, formado em Análise e Desenvolvimento de Sistemas e
pós-graduado em **Engenharia de Software pela PUC-Rio**. Concluí a especialização
**Oracle Next Education (ONE)** em backend com Java e Spring Boot.

> Vim do **suporte técnico**, e isso mudou como eu escrevo código: aprendi a
> diagnosticar sistema quebrado com usuário esperando do outro lado, e trago essa
> cabeça para as decisões de arquitetura.

Hoje trabalho com **APIs REST, arquitetura em camadas e microsserviços**.

## Stack

<div align="center">

**Back-end e dados**

[![Back-end](https://skillicons.dev/icons?i=java,spring,python,django,postgres,mysql,mongodb&theme=dark)](https://skillicons.dev)

**Front-end e ferramentas**

[![Ferramentas](https://skillicons.dev/icons?i=react,nextjs,ts,docker,git,github,postman&theme=dark)](https://skillicons.dev)

</div>

**Também aplico no dia a dia:** APIs REST · Microsserviços · Clean Code · SOLID ·
Arquitetura em camadas · Integração com APIs externas · Tratamento de exceções

## Projetos em destaque

<div align="center">

<a href="https://github.com/eliel2107/mvp-apigateway-nasa-java">
  <img width="49%" src="https://github-readme-stats.vercel.app/api/pin/?username=eliel2107&repo=mvp-apigateway-nasa-java&theme=tokyonight&hide_border=true&title_color=70A5FD&icon_color=BB9AF7" />
</a>
<a href="https://github.com/eliel2107/mvp-api-observacoesnasa-java">
  <img width="49%" src="https://github-readme-stats.vercel.app/api/pin/?username=eliel2107&repo=mvp-api-observacoesnasa-java&theme=tokyonight&hide_border=true&title_color=70A5FD&icon_color=BB9AF7" />
</a>
<a href="https://github.com/eliel2107/Challenge-ApiRestForumHub">
  <img width="49%" src="https://github-readme-stats.vercel.app/api/pin/?username=eliel2107&repo=Challenge-ApiRestForumHub&theme=tokyonight&hide_border=true&title_color=70A5FD&icon_color=BB9AF7" />
</a>
<a href="https://github.com/eliel2107/Challenge-LiterAlura">
  <img width="49%" src="https://github-readme-stats.vercel.app/api/pin/?username=eliel2107&repo=Challenge-LiterAlura&theme=tokyonight&hide_border=true&title_color=70A5FD&icon_color=BB9AF7" />
</a>

</div>

### NASA Observações — três serviços, um sistema

MVP de arquitetura em microsserviços: **só o gateway conhece as APIs públicas da
NASA** — o front nunca fala com elas direto. Os dois serviços em Java sobem com
Docker e documentam as rotas em Swagger.

```mermaid
flowchart LR
    F(["Front-end<br/>Next.js · React · TypeScript"])
    G(["API Gateway<br/>Java 21 · Spring Boot"])
    O(["API de Observações<br/>Java · Spring Boot · PostgreSQL"])
    N(["APIs públicas da NASA<br/>Hubble · APOD"])

    F -- "busca de imagens e APOD" --> G
    F -- "coleções e itens" --> O
    G --> N

    classDef meu fill:#1A1B27,stroke:#70A5FD,stroke-width:2px,color:#C0CAF5
    classDef externo fill:#24283B,stroke:#BB9AF7,stroke-width:2px,color:#C0CAF5
    class F,G,O meu
    class N externo
```

| Serviço | O que faz | Stack |
| --- | --- | --- |
| **[API Gateway](https://github.com/eliel2107/mvp-apigateway-nasa-java)** | Porta de entrada única: busca imagens do Hubble, serve a foto astronômica do dia (APOD, inclusive por intervalo de datas) e repassa a gestão de coleções ao serviço de observações. | ![Java 21](https://img.shields.io/badge/Java_21-ED8B00?style=flat-square&logo=openjdk&logoColor=white) ![Spring Boot](https://img.shields.io/badge/Spring_Boot_3.3-6DB33F?style=flat-square&logo=springboot&logoColor=white) |
| **[API de Observações](https://github.com/eliel2107/mvp-api-observacoesnasa-java)** | Persiste coleções e itens em PostgreSQL, com migrations em Flyway. Não conhece a NASA: só guarda o que o usuário colecionou. | ![Java 21](https://img.shields.io/badge/Java_21-ED8B00?style=flat-square&logo=openjdk&logoColor=white) ![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white) ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white) |
| **[Front-end](https://github.com/eliel2107/mvp-frontend-nasa)** | Interface para buscar imagens, ver o APOD e montar coleções de observações. | ![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white) ![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=1A1B27) ![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white) |

### Outros projetos

| Projeto | O que é | Stack |
| --- | --- | --- |
| **[ForumHub API](https://github.com/eliel2107/Challenge-ApiRestForumHub)** | API REST de tópicos de fórum, com CRUD completo em Spring Boot. | ![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white) ![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white) |
| **[LiterAlura](https://github.com/eliel2107/Challenge-LiterAlura)** | Consome a API Gutendex para buscar livros e explorar autores. | ![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white) |
| **[MVP Microsserviços](https://github.com/eliel2107/MVP-microservicos)** | A primeira versão da arquitetura, na pós da PUC-Rio. | ![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white) ![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white) |
| **[ProjetoIA](https://github.com/eliel2107/ProjetoIA)** | Aplicação interativa com Streamlit e LangChain. | ![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white) |

## GitHub

<div align="center">

<img height="170" src="https://github-readme-stats.vercel.app/api?username=eliel2107&show_icons=true&theme=tokyonight&hide_border=true&include_all_commits=true&title_color=70A5FD&icon_color=BB9AF7" />
<img height="170" src="https://github-readme-stats.vercel.app/api/top-langs/?username=eliel2107&layout=compact&theme=tokyonight&hide_border=true&langs_count=8&title_color=70A5FD" />

<img height="170" src="https://streak-stats.demolab.com?user=eliel2107&theme=tokyonight&hide_border=true&ring=70A5FD&fire=BB9AF7&currStreakLabel=70A5FD" />

<img width="98%" src="https://github-readme-activity-graph.vercel.app/graph?username=eliel2107&theme=tokyo-night&hide_border=true&area=true&custom_title=Atividade%20recente&title_color=70A5FD&line=70A5FD&point=BB9AF7&color=C0CAF5" />

</div>

<!--
A cobrinha das contribuicoes ja esta pronta em .github/workflows/main.yml, mas o
workflow esta desativado. Para ligar: aba Actions > "Gera a cobrinha das
contribuicoes" > Enable workflow > Run workflow. Depois que a branch output
aparecer, e so descomentar o bloco abaixo.

<div align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/eliel2107/eliel2107/output/github-contribution-grid-snake-dark.svg" />
    <img alt="" src="https://raw.githubusercontent.com/eliel2107/eliel2107/output/github-contribution-grid-snake.svg" />
  </picture>
</div>
-->

<div align="center">

### Aberto a oportunidades como Desenvolvedor Back-End

<a href="https://www.linkedin.com/in/eliel-mesquita0799/"><img alt="Vamos conversar" src="https://img.shields.io/badge/Vamos_conversar-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" /></a>

<img width="100%" alt="" src="https://capsule-render.vercel.app/api?type=waving&color=0:70A5FD,45:414868,100:1A1B27&height=130&section=footer" />

</div>
