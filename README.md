<!--
  Os arquivos de imagem citados aqui (pacora-*.png, shot-*.png e demo-*.gif)
  ficam na pasta pacora-readme-arquivos, ao lado deste README.
-->

<div align="center">

<img src="./pacora-readme-arquivos/pacora-banner.png" alt="Pacora, gestor de turmas" width="100%" />

<br/><br/>

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="./pacora-readme-arquivos/pacora-logo-dark.png">
  <img src="./pacora-readme-arquivos/pacora-logo.png" alt="Pacora" width="360">
</picture>

<br/><br/>

**Turmas, grupos, notas e relatórios em um só lugar.**
<br/>
Um sistema para o representante de turma organizar a semana inteira, de segunda a sábado.

<br/>

<img src="https://img.shields.io/badge/React-18-0A1F5C?style=for-the-badge&logo=react&logoColor=61DAFB" alt="React" />
<img src="https://img.shields.io/badge/Supabase-Auth%20%2B%20Postgres-0A1F5C?style=for-the-badge&logo=supabase&logoColor=3ECF8E" alt="Supabase" />
<img src="https://img.shields.io/badge/Chart.js-gr%C3%A1ficos-0A1F5C?style=for-the-badge&logo=chartdotjs&logoColor=FF6384" alt="Chart.js" />
<img src="https://img.shields.io/badge/Arquivo%20%C3%BAnico-sem%20build-1D4FD8?style=for-the-badge&logo=html5&logoColor=white" alt="Arquivo único" />

<br/><br/>

[Sobre](#sobre) &nbsp;|&nbsp; [O sistema em uso](#o-sistema-em-uso) &nbsp;|&nbsp; [Recursos](#recursos) &nbsp;|&nbsp; [Acesso e permissões](#acesso-e-permissões) &nbsp;|&nbsp; [Publicar](#como-publicar) &nbsp;|&nbsp; [Banco de dados](#banco-de-dados)

</div>

<br/>

## Sobre

A **Pacora** é uma central de controle para o representante administrar as **6 turmas da semana**. Em vez de planilhas e anotações soltas, tudo fica em um só lugar: grupos dinâmicos, alunos, líderes, três tipos de nota, diário de ocorrências, relatórios em PDF e um registro de tudo que foi alterado.

O sistema é um único arquivo `index.html`. Não tem instalação nem etapa de build: basta publicar o arquivo e conectar um projeto Supabase gratuito.

<table>
<tr>
<td width="33%" valign="top">

**Organizado**

Turmas de segunda a sábado, grupos que podem ser reorganizados por arrastar e soltar, líderes e representantes em destaque.

</td>
<td width="33%" valign="top">

**Justo**

Nota individual, nota individual do grupo e nota do grupo ficam separadas. A média do grupo usa só a nota individual do grupo.

</td>
<td width="33%" valign="top">

**Seguro**

Login por usuário, dois níveis de acesso, regras de segurança no banco e registro de atividades visível apenas ao administrador.

</td>
</tr>
</table>

<br/>

## O sistema em uso

### Visão geral e grupos

<div align="center">
<img src="./pacora-readme-arquivos/demo-tour.gif" alt="Navegando pelo dashboard, pela turma e reorganizando grupos com arrastar e soltar" width="92%" />
<br/><sub>Dashboard, turma da segunda-feira e quadro de grupos com arrastar e soltar.</sub>
</div>

<br/>

### Notas e média do grupo

<div align="center">
<img src="./pacora-readme-arquivos/demo-notas.gif" alt="Lançando notas individuais do grupo e calculando a média do grupo" width="92%" />
<br/><sub>Notas individuais do grupo lançadas dentro do grupo e cálculo automático da média (quem não tem nota conta zero).</sub>
</div>

<br/>

### Todos os alunos

<div align="center">
<img src="./pacora-readme-arquivos/demo-alunos.gif" alt="Busca e filtros na listagem de todos os alunos" width="92%" />
<br/><sub>Listagem geral em ordem alfabética, com busca por nome ou RGM e filtros por dia e grupo.</sub>
</div>

<br/>

### Tema escuro e tema claro

<div align="center">
<img src="./pacora-readme-arquivos/demo-tema.gif" alt="Alternando entre o tema escuro e o tema claro" width="92%" />
<br/><sub>O padrão é o azul-marinho com degradê royal. Um botão muda para o tema claro.</sub>
</div>

<br/>

### No celular

<div align="center">
<img src="./pacora-readme-arquivos/demo-celular.gif" alt="Sistema no celular, com barra de navegação inferior" width="300" />
<br/><sub>Barra de navegação inferior, tabelas em cartões e janelas que abrem de baixo para cima.</sub>
</div>

<br/>

### Capturas de tela

<table>
<tr>
<td width="50%"><img src="./pacora-readme-arquivos/shot-dashboard.png" alt="Dashboard" /><br/><sub>Dashboard</sub></td>
<td width="50%"><img src="./pacora-readme-arquivos/shot-turma.png" alt="Grupos da turma" /><br/><sub>Grupos da turma</sub></td>
</tr>
<tr>
<td width="50%"><img src="./pacora-readme-arquivos/shot-notas.png" alt="Notas do grupo" /><br/><sub>Notas do grupo</sub></td>
<td width="50%"><img src="./pacora-readme-arquivos/shot-alunos.png" alt="Todos os alunos" /><br/><sub>Todos os alunos</sub></td>
</tr>
<tr>
<td width="50%"><img src="./pacora-readme-arquivos/shot-claro.png" alt="Tema claro" /><br/><sub>Tema claro</sub></td>
<td width="50%" align="center"><img src="./pacora-readme-arquivos/shot-celular.png" alt="Versão para celular" width="45%" /><br/><sub>Celular</sub></td>
</tr>
</table>

<sub>As capturas usam os dados de exemplo do próprio sistema, por isso aparece o aviso de dados demonstrativos.</sub>

<br/>

## Recursos

<table>
<tr>
<td width="50%" valign="top">

### Turmas e pessoas

- 6 turmas fixas, cada uma com quantidade própria de grupos
- Grupos em ordem natural (G1, G2 ... G10) e alunos em ordem alfabética
- Alunos com nome, RGM e histórico de grupos
- Líder de grupo e representantes de turma
- Listagem **Todos os alunos** com busca e filtros
- Onde a professora está e calendário de eventos

</td>
<td width="50%" valign="top">

### Notas e diário

- **Nota individual**, **nota individual do grupo** e **nota do grupo**
- Notas lançadas, editadas e removidas com confirmação
- Lançamento das notas dos integrantes direto no card do grupo
- Média do grupo calculada pelas notas individuais do grupo
- Diário da turma e do grupo, com edição dos registros

</td>
</tr>
<tr>
<td width="50%" valign="top">

### Relatórios

- PDF por turma, grupo ou aluno, com a logo da Pacora
- As três notas aparecem separadas e a regra da média vem explicada
- Tabela de grupos com a média e a nota coletiva
- Alunos sempre em ordem alfabética

</td>
<td width="50%" valign="top">

### Administração

- Painel do administrador com usuários, convites e conexão
- Registro de atividades: quem lançou, editou ou apagou cada nota
- Tema escuro e claro, com a escolha salva
- Layout pensado para celular

</td>
</tr>
</table>

### Regra das notas

```mermaid
flowchart LR
    A[Nota individual do aluno] -->|não entra na média| X[ ]
    B[Nota individual do grupo<br/>de cada integrante] --> M[Média do grupo]
    M --> G[Nota do grupo]
    style X fill:none,stroke:none
    style M fill:#1D4FD8,stroke:#3D7BFF,color:#ffffff
```

A média do grupo soma a nota individual do grupo de cada integrante e divide pelo total de integrantes. Quem não tem nota lançada conta como 0. A nota individual do aluno é uma avaliação à parte e não participa dessa conta.

<br/>

## Acesso e permissões

O acesso é feito por login, com dois níveis:

| Nível | O que pode fazer |
| --- | --- |
| **Administrador** | Tudo o que o representante faz, mais o painel do ADM: convidar e gerenciar usuários, configurar a conexão, sincronizar, consultar o registro de atividades e usar **Apagar os dados** |
| **Representante** | Gerenciar turmas, alunos, grupos, notas e diário. Não vê o painel e não apaga os dados do sistema |

**Convite com senha própria.** O administrador gera um convite com um link. O usuário abre o link, confere o e-mail e o código e cria a própria senha. Ninguém vê a senha, nem o administrador.

**Conexão embutida.** O administrador configura a URL e a chave `anon` uma única vez e baixa pelo painel um `index.html` com a conexão embutida. Depois de publicado, os usuários só digitam e-mail e senha.

<br/>

## Como publicar

1. Crie um projeto gratuito no [Supabase](https://supabase.com) e rode o `schema.sql` no **SQL Editor**.
2. Publique o `index.html` em qualquer hospedagem estática (GitHub Pages, Netlify, Vercel).
3. Crie o primeiro usuário em **Authentication, Users** (ele vira administrador) e entre pelo endereço publicado.
4. No **Painel do ADM**, gere o arquivo com a conexão embutida, publique-o no lugar do atual e convide os representantes.

Para testar sem banco, o sistema também tem um modo local, com dados de exemplo opcionais, que salva apenas no navegador.

<br/>

## Banco de dados

O `schema.sql` cria as tabelas, os perfis de acesso, o registro de atividades e as políticas de segurança (RLS). A chave `anon` não é uma credencial de administrador, e a chave `service_role` nunca é usada no navegador.

```mermaid
erDiagram
    classes ||--o{ groups : possui
    classes ||--o{ students : possui
    groups ||--o{ students : reune
    students ||--o{ individual_grades : recebe
    groups ||--o{ group_grades_history : recebe
    classes ||--o{ diary_entries : registra
    profiles ||--o{ audit_log : gera
    invites }o--|| profiles : origina
```

| Tabela | Função |
| --- | --- |
| `classes`, `groups`, `students` | Turmas, grupos e alunos |
| `individual_grades` | Notas individuais e notas individuais do grupo (campo `kind`) |
| `group_grades_history` | Histórico da nota coletiva do grupo |
| `diary_entries`, `events` | Diário de bordo e calendário |
| `profiles`, `invites` | Usuários, níveis de acesso e convites |
| `audit_log` | Registro de atividades, legível apenas pelo administrador |

<br/>

## Tecnologias

<div align="center">
<img src="https://skillicons.dev/icons?i=html,css,js,react,supabase,postgres,git,github&theme=dark" alt="Tecnologias utilizadas" />
</div>

<br/>

## Autor

<div align="center">

**Cicero Kaue Alves da Silva**
<br/>
Estudante de Engenharia de Software

<a href="https://github.com/callmekaue">
  <img src="https://img.shields.io/badge/GitHub-callmekaue-0A1F5C?style=for-the-badge&logo=github&logoColor=white" alt="GitHub" />
</a>

</div>
