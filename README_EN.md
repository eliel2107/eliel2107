<div align="center">

<img width="100%" alt="" src="https://capsule-render.vercel.app/api?type=waving&color=0:1A1B27,55:414868,100:70A5FD&height=200&section=header&text=Eliel%20Mesquita&fontSize=50&fontColor=FFFFFF&fontAlignY=34&desc=Back-End%20Developer%20%20%7C%20%20Java%20%C2%B7%20Spring%20Boot%20%C2%B7%20Python&descAlignY=55&descSize=16" />

<a href="./README.md"><img alt="Português" src="https://img.shields.io/badge/Portugu%C3%AAs-24283B?style=flat-square&labelColor=1A1B27" /></a>
<a href="./README_EN.md"><img alt="English" src="https://img.shields.io/badge/English-70A5FD?style=flat-square&labelColor=1A1B27" /></a>

[![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=21&pause=1200&color=70A5FD&center=true&vCenter=true&width=560&height=45&lines=REST+APIs+in+Java+and+Spring+Boot;Layered+architecture+and+microservices;From+technical+support+to+the+back+end)](https://github.com/eliel2107)

<a href="https://www.linkedin.com/in/eliel-mesquita0799/"><img alt="LinkedIn" src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" /></a>
<a href="mailto:eliel.mesquita@gmail.com"><img alt="Gmail" src="https://img.shields.io/badge/Gmail-EA4335?style=for-the-badge&logo=gmail&logoColor=white" /></a>

</div>

## About me

**Back-End developer** with a degree in Systems Analysis and Development and a
**postgraduate degree in Software Engineering from PUC-Rio**. I completed the
**Oracle Next Education (ONE)** backend specialization in Java and Spring Boot.

> I came from **technical support**, and it changed how I write code: I learned to
> diagnose a broken system with a user waiting on the other end, and I bring that
> mindset to architecture decisions.

Today I work with **REST APIs, layered architecture and microservices**.

## Stack

<div align="center">

**Back end and data**

[![Back end](https://skillicons.dev/icons?i=java,spring,python,django,postgres,mysql,mongodb&theme=dark)](https://skillicons.dev)

**Front end and tooling**

[![Tooling](https://skillicons.dev/icons?i=react,nextjs,ts,docker,git,github,postman&theme=dark)](https://skillicons.dev)

</div>

**Also part of my day-to-day:** REST APIs · Microservices · Clean Code · SOLID ·
Layered architecture · Third-party API integration · Exception handling

## Featured projects

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

### NASA Observations — three services, one system

A microservices MVP: **only the gateway knows NASA's public APIs** — the front
end never calls them directly. Both Java services ship with Docker and document
their routes in Swagger.

```mermaid
flowchart LR
    F(["Front end<br/>Next.js · React · TypeScript"])
    G(["API Gateway<br/>Java 21 · Spring Boot"])
    O(["Observations API<br/>Java · Spring Boot · PostgreSQL"])
    N(["NASA public APIs<br/>Hubble · APOD"])

    F -- "imagery and APOD lookups" --> G
    F -- "collections and items" --> O
    G --> N

    classDef mine fill:#1A1B27,stroke:#70A5FD,stroke-width:2px,color:#C0CAF5
    classDef external fill:#24283B,stroke:#BB9AF7,stroke-width:2px,color:#C0CAF5
    class F,G,O mine
    class N external
```

| Service | What it does | Stack |
| --- | --- | --- |
| **[API Gateway](https://github.com/eliel2107/mvp-apigateway-nasa-java)** | Single entry point: searches Hubble imagery, serves the Astronomy Picture of the Day (including date ranges) and forwards collection management to the observations service. | ![Java 21](https://img.shields.io/badge/Java_21-ED8B00?style=flat-square&logo=openjdk&logoColor=white) ![Spring Boot](https://img.shields.io/badge/Spring_Boot_3.3-6DB33F?style=flat-square&logo=springboot&logoColor=white) |
| **[Observations API](https://github.com/eliel2107/mvp-api-observacoesnasa-java)** | Persists collections and items in PostgreSQL, with Flyway migrations. It knows nothing about NASA: it just stores what the user collected. | ![Java 21](https://img.shields.io/badge/Java_21-ED8B00?style=flat-square&logo=openjdk&logoColor=white) ![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white) ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white) |
| **[Front end](https://github.com/eliel2107/mvp-frontend-nasa)** | Interface to search imagery, browse the APOD and build observation collections. | ![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white) ![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=1A1B27) ![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white) |

### Other projects

| Project | What it is | Stack |
| --- | --- | --- |
| **[ForumHub API](https://github.com/eliel2107/Challenge-ApiRestForumHub)** | REST API for forum topics, full CRUD in Spring Boot. | ![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white) ![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white) |
| **[LiterAlura](https://github.com/eliel2107/Challenge-LiterAlura)** | Consumes the Gutendex API to search books and explore authors. | ![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white) |
| **[MVP Microservices](https://github.com/eliel2107/MVP-microservicos)** | The first take on the architecture, during the PUC-Rio program. | ![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white) ![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white) |
| **[ProjetoIA](https://github.com/eliel2107/ProjetoIA)** | Interactive application built with Streamlit and LangChain. | ![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white) |

## GitHub

<div align="center">

<img height="170" src="https://github-readme-stats.vercel.app/api?username=eliel2107&show_icons=true&theme=tokyonight&hide_border=true&include_all_commits=true&title_color=70A5FD&icon_color=BB9AF7" />
<img height="170" src="https://github-readme-stats.vercel.app/api/top-langs/?username=eliel2107&layout=compact&theme=tokyonight&hide_border=true&langs_count=8&title_color=70A5FD" />

<img height="170" src="https://streak-stats.demolab.com?user=eliel2107&theme=tokyonight&hide_border=true&ring=70A5FD&fire=BB9AF7&currStreakLabel=70A5FD" />

<img width="98%" src="https://github-readme-activity-graph.vercel.app/graph?username=eliel2107&theme=tokyo-night&hide_border=true&area=true&custom_title=Recent%20activity&title_color=70A5FD&line=70A5FD&point=BB9AF7&color=C0CAF5" />

</div>

<!--
The contribution snake is already wired up in .github/workflows/main.yml, but the
workflow is disabled. To turn it on: Actions tab > "Gera a cobrinha das
contribuicoes" > Enable workflow > Run workflow. Once the output branch shows up,
uncomment the block below.

<div align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/eliel2107/eliel2107/output/github-contribution-grid-snake-dark.svg" />
    <img alt="" src="https://raw.githubusercontent.com/eliel2107/eliel2107/output/github-contribution-grid-snake.svg" />
  </picture>
</div>
-->

<div align="center">

### Open to Back-End Developer opportunities

<a href="https://www.linkedin.com/in/eliel-mesquita0799/"><img alt="Let's talk" src="https://img.shields.io/badge/Let's_talk-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" /></a>

<img width="100%" alt="" src="https://capsule-render.vercel.app/api?type=waving&color=0:70A5FD,45:414868,100:1A1B27&height=130&section=footer" />

</div>
