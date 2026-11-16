<!-- ===================================================================== -->
<!--  Troque SEU_USUARIO pelo seu usuário do GitHub (Ctrl+H no editor).    -->
<!--  Envie também a pasta assets/ e o arquivo .github/workflows/snake.yml -->
<!-- ===================================================================== -->

<p align="center">
  <img src="./assets/banner.svg" width="100%" alt="Isaque Santos Bomfim — Arquitetura de Software, Launchers e Infraestrutura" />
</p>

## `01` Sobre mim

Estudante de **Engenharia de Software** com foco em **arquitetura de software**, **launchers** e **infraestrutura**.

Gosto de olhar para o sistema inteiro: como o código se organiza por dentro, como ele chega até a máquina de quem usa e como continua atualizado depois disso.

Minha base vem de Ciência da Computação, com o **CS50 de Harvard** e o **Computer Science** da Codecademy, e de formações em **Java**, **AWS**, **Microsoft Azure** e **Red Hat**.

- Atualmente programo em **C#, Java, C++ e JavaScript**
- Uso bancos **relacionais** (MySQL, PostgreSQL) e **NoSQL** (MongoDB)
- Estudo **cloud** na **AWS** e na **Azure**
- Meta: transformar ideias em projetos.

```csharp
public sealed class IsaqueSantosBomfim
{
    public string   Status        => "Estudante de Engenharia de Software";
    public string[] Foco          => ["Arquitetura de Software", "Launchers", "Infraestrutura"];

    public string[] Linguagens    => ["C#", "Java", "C++", "JavaScript"];
    public string[] BancosDeDados => ["MySQL", "PostgreSQL", "MongoDB"];
    public string[] Cloud         => ["AWS", "Azure"];

    public string   Meta          => "Transformar ideias em projetos.";
}
```

<img src="./assets/divider.svg" width="100%" alt="" />

## `02` Onde eu foco

<table>
<tr>
<th width="33%" align="left">Arquitetura de Software</th>
<th width="33%" align="left">Launchers</th>
<th width="33%" align="left">Infraestrutura</th>
</tr>
<tr>
<td valign="top">

Sistemas organizados em camadas e módulos, cada um com uma responsabilidade clara.

<sub>Orientação a objetos · padrões de projeto · código fácil de manter e de evoluir</sub>

</td>
<td valign="top">

Aplicações que distribuem, atualizam e iniciam outros softwares do jeito certo.

<sub>Controle de versões · download de pacotes · verificação de integridade · atualização automática</sub>

</td>
<td valign="top">

O caminho que o software percorre do código até rodar na máquina do usuário.

<sub>Cloud na AWS e na Azure · bancos relacionais e NoSQL · build e distribuição</sub>

</td>
</tr>
</table>

### Como eu penso um launcher

Cada parte faz uma coisa só: o launcher pergunta, a nuvem responde, e nada é executado antes de ser verificado.

```mermaid
sequenceDiagram
    autonumber
    actor U as Usuário

    box rgba(56, 189, 248, 0.08) Máquina do usuário
        participant L as Launcher
    end

    box rgba(56, 189, 248, 0.16) Cloud · AWS / Azure
        participant A as API de versões
        participant D as Banco de dados
        participant S as Storage de pacotes
    end

    U->>L: abre o launcher
    L->>A: existe versão nova?
    A->>D: consulta a versão atual
    D-->>A: versão + hashes dos arquivos
    A-->>L: sim, aqui está o manifesto
    L->>S: baixa os pacotes
    S-->>L: pacotes
    L->>L: confere a integridade (hash)

    alt pacotes íntegros
        L->>U: inicia a aplicação
    else arquivo corrompido
        L->>S: baixa de novo
    end
```

<img src="./assets/divider.svg" width="100%" alt="" />

## `03` Stack

<table>
<tr>
<th align="center">Linguagens</th>
<th align="center">Bancos de Dados</th>
<th align="center">Cloud</th>
<th align="center">Versionamento</th>
</tr>
<tr>
<td align="center"><img src="https://skillicons.dev/icons?i=cs,java,cpp,js&perline=2" alt="C#, Java, C++, JavaScript" /></td>
<td align="center"><img src="https://skillicons.dev/icons?i=mysql,postgres,mongodb&perline=2" alt="MySQL, PostgreSQL, MongoDB" /></td>
<td align="center"><img src="https://skillicons.dev/icons?i=aws,azure&perline=1" alt="AWS, Azure" /></td>
<td align="center"><img src="https://skillicons.dev/icons?i=git,github&perline=1" alt="Git, GitHub" /></td>
</tr>
</table>

<img src="./assets/divider.svg" width="100%" alt="" />

## `04` Formação

| Trilha | Onde estudei |
| :-- | :-- |
| **Fundamentos de Computação** | HarvardX · CS50: Introduction to Computer Science<br/>Codecademy · Computer Science |
| **Java** | W3Schools · Java Professional |
| **Cloud** | AWS Skill Builder<br/>Microsoft Azure |
| **Infraestrutura** | Red Hat |
| **Complementares** | Coursera · Google · HackerRank · Fundação Bradesco |

<img src="./assets/divider.svg" width="100%" alt="" />

## `05` GitHub

<p align="center">
  <img height="165" src="https://github-profile-summary-cards.vercel.app/api/cards/stats?username=https://github.com/Nordic0x00&theme=github_dark" alt="Estatísticas do GitHub" />
  <img height="165" src="https://github-profile-summary-cards.vercel.app/api/cards/most-commit-language?username=https://github.com/Nordic0x00&theme=github_dark" alt="Linguagens mais usadas" />
</p>

<p align="center">
  <img src="https://streak-stats.demolab.com?user=SEU_USUARIO&locale=pt_BR&background=0D1117&border=30363D&stroke=30363D&ring=38BDF8&fire=38BDF8&currStreakNum=E6EDF3&sideNums=E6EDF3&currStreakLabel=38BDF8&sideLabels=8B949E&dates=6E7681" alt="Sequência de contribuições" />
</p>

<p align="center">
  <img width="100%" src="https://github-readme-activity-graph.vercel.app/graph?username=SEU_USUARIO&bg_color=0D1117&color=8B949E&title_color=E6EDF3&line=38BDF8&point=E6EDF3&area=true&area_color=38BDF8&hide_border=false&border_color=30363D&custom_title=Contribui%C3%A7%C3%B5es%20nos%20%C3%BAltimos%2031%20dias" alt="Gráfico de contribuições" />
</p>

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/SEU_USUARIO/SEU_USUARIO/output/github-snake-dark.svg" />
    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/SEU_USUARIO/SEU_USUARIO/output/github-snake.svg" />
    <img alt="Animação percorrendo o gráfico de contribuições" src="https://raw.githubusercontent.com/SEU_USUARIO/SEU_USUARIO/output/github-snake.svg" />
  </picture>
</p>

<!-- ===================================================================== -->
<!--  CONTATO (escondido): para mostrar, apague a primeira e a última      -->
<!--  linha do bloco abaixo e troque SEU_LINKEDIN e SEU_EMAIL.            -->
<!-- ===================================================================== -->

<!--
<img src="./assets/divider.svg" width="100%" alt="" />

## `06` Contato

<p align="left">
  <a href="https://www.linkedin.com/in/SEU_LINKEDIN"><img src="https://img.shields.io/badge/LinkedIn-0D1117?style=for-the-badge&logo=linkedin&logoColor=38BDF8" alt="LinkedIn" /></a>
  <a href="mailto:SEU_EMAIL"><img src="https://img.shields.io/badge/E--mail-0D1117?style=for-the-badge&logo=gmail&logoColor=38BDF8" alt="E-mail" /></a>
</p>
-->

<img src="./assets/divider.svg" width="100%" alt="" />

<p align="center">
  <sub>Valeu pela visita. Se algo aqui chamou sua atenção, deixe uma estrela nos meus repositórios.</sub>
</p>
