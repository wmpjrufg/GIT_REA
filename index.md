---
title: Seja bem-vindo!
layout: home
nav_order: 1
---

<h1>O que vamos ver?!</h1>

<p align = "justify">
Este é o curso de Git e GitHub e tem como objetivo central oferecer aos alunos uma introdução a gestão de códigos usando a plataforma Git e GitHub.<br><br>

Este curso é ministrado foi produzido pelo Grupo de Pesquisa e Estudos em Engenharia (GPEE) que é liderado pelo professor  <a href="http://lattes.cnpq.br/2268506213083114" target = "_blank" rel = "noopener noreferrer">Wanderlei Malaquias Pereira Junior</a>.<br><br>

Este espaço será destinado a apresentação do seguinte conteúdo:
</p>

<table>
  <tr>
    <td style = "width:70%;">
        <ol>
            <li>Configurações e primeiros passos;</li>
            <li>Git e Git Hub na prática;</li>
            <li>Boas pŕaticas;</li>
            <li>Desafio;</li>
        </ol>
    </td>
    <td style = "width:30%;"><center><img src = "assets/images/fig00.png" width = "60%"></center></td>
  </tr>
</table>

<p align = "justify">
Vamos iniciar o curso pela instalação dos recursos necessários para uso do Git em um computador seja ele Linux ou Windows. Vamos instalar os seguintes programas:<br>
</p>

<ol>
    <li><a href = "https://git-scm.com/">Plataforma Git</a>;</li>
    <li><a href = "https://code.visualstudio.com">Visual Studio Code</a>;</li>
</ol>

<p align = "justify">
Após a instalação é necessário criar uma conta no repositório <i>online</i> <a href = "https://github.com/">GitHub</a>.
</p>

{: .highlight-title }
> Testando o git
>
> Para verificar se o git foi instalado corretamente vá até o terminal e digite o seguinte comando: `git --version`.Provavelmente após a execução aparecerá no terminal a versão do git, por exemplo: `git version 2.34.1`.

<p align = "justify">
Após o comando mostrado acima você pode verificar se o Git foi instalado corretamente no Visual Studio Code conforme a <a href = "#fig04">Figura 0.1</a>.  
</p>

<p align = "left" id = "fig04"><b>Figura 0.1</b> Verificação do Git no Visual Studio Code.</p>
<center><img src = "assets/images/fig04.png" width = "100%"></center>

<h1>O conceito de controle de versão</h1>

<p align = "justify">
O Git é um <i>software</i> de gerenciamento de versão em documentos. Essa temática é um braço da engenharia de <i>software</i> que consiste em uma junção de técnicas para rastrear e controlar alterações sobre um código ou conjunto de códigos.
<br><br>
Um controle de versão simplificado poderia ser por representado por um usuário mudando o nome do arquivo a medida que o mesmo fosse evoluindo. Um exemplo dessa mudança de nomenclatura em um documento pode ser visto a seguir.
</p>

```cmd
├── ...
├── diretorio               
│   ├── arquivo_20230824.py   # Arquivo salvo no dia 24-08-2023
│   ├── arquivo_20230825.py   # Arquivo salvo no dia 25-08-2023
│   └── arquivo_20230912.py   # Arquivo salvo no dia 12-09-2023
└── ...
```

{: .note }
> Com o Git vamos fazer esse controle de forma mais eficiente e automatizada garantindo sempre que todas as etapas sejam rastreadas.

<p align = "justify">
A <a href = "#fig02">Figura 0.2</a> apresenta algumas ferramentas que controlam a revisão de código e nesse curso o foco será dado para ferramenta Git.
</p>

<table>
<thead>
  <tr>
    <td><center><img src="assets/images/fig01.png" width="60%"></center></td>
    <td><center><img src="assets/images/fig02.png" width="60%"></center></td>
    <td><center><img src="assets/images/fig03.svg" width="600%"></center></td>
  </tr>
</thead>
</table>
<p align = "center" id = "fig02"><b>Figura 0.2</b> Plataformas de controle de versão.</p>

<h1>O que é Git e por que ele é usado?</h1>

<p align = "justify">
Git é um sistema de controle de versão distribuído, e serve para facilitar a edição do código-fonte de um projeto por múltiplos usuários de forma simultânea sem que as alterações sobrescrevam outras, e caso haja edições no mesmo local de um repositório (nome dado ao diretório de um projeto), por exemplo, o controle de versão armazena todo o histórico de alterações, sendo possível retornar à versão anterior do projeto, ou seja, à última vez em que ele foi salvo. Além disso, é possível saber que alterações foram feitas no projeto e por quem, o que facilita o controle.
</p>

{: .note }
> Git e GitHub são conceitos diferentes. O GitHub é uma plataforma <i>web</i> que utiliza a o Git como <i>framework</i> controlador de versão.