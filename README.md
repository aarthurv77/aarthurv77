<p align="center">
  <img src="https://capsule-render.vercel.app/api?text=Olá, Eu sou o Arthur!&animation=fadeIn&type=waving&color=gradient&height=100"/>
</p>

### 👨‍💻 About Me

```javascript
const arthur = {
    name: "Arthur Vargas",
    located_in: "Brasília, Brazil",
    current_job: "Data Analyst",
    education: [
        "Bachelor's Computer Science @ University of Brasília (UnB)",
    ],
    company: "ADASA"

    fields_of_interest: [
        "Web Development",
        "UI/UX",
        "Back-end",
        "Machine Learning",
        "Data Science",
        "Cloud Computing",
        "Competitive Programming",
    ],

    technical_background: [
        "C++ (OOP Systems)",
        "Power BI & Power Plataform",
        "Python for Data Science",
    ],

    current_learning: [
        "Java (Spring Boot)",
        "React Native",
        "AWS Cloud",
    ],

    hobbies: [
        "Reading", 
        "Sports", 
        "Cinema",
        "Jiu-Jitsu"
    ]
};

<p align="left">
  <img src="[https://cdn.jsdelivr.net/gh/devicons/devicon/icons/java/java-original.svg](https://cdn.jsdelivr.net/gh/devicons/devicon/icons/java/java-original.svg)" width="40" height="40"/>
  <img src="[https://cdn.jsdelivr.net/gh/devicons/devicon/icons/spring/spring-original.svg](https://cdn.jsdelivr.net/gh/devicons/devicon/icons/spring/spring-original.svg)" width="40" height="40"/>
  <img src="[https://cdn.jsdelivr.net/gh/devicons/devicon/icons/docker/docker-original.svg](https://cdn.jsdelivr.net/gh/devicons/devicon/icons/docker/docker-original.svg)" width="40" height="40"/>
</p>

![Estatísticas do Arthur](https://github-readme-stats.vercel.app/api?username=SEU_USUARIO&show_icons=true&theme=dracula)

name: Generate Snake

on:
  schedule:
    - cron: "0 */12 * * *" # Roda a cada 12 horas
  workflow_dispatch:

jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v2
      
      - uses: Platane/snk@master
        id: snake-gif
        with:
          github_user_name: SEU_USUARIO_AQUI
          svg_out_path: dist/github-contribution-grid-snake.svg

      - uses: crazy-max/ghaction-github-pages@v2.1.3
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}


![Snake animation](https://github.com/aarthurv77/aarthurv77/blob/output/github-contribution-grid-snake.svg)
