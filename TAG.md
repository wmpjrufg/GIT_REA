---
layout: default
title: Guardando versão
nav_order: 6
parent: Git e GitHub na prática
---

<p align = "justify">
  Na plataforma git hub é possível registrar ou especificar pontos do algoritmo que achamos importantes, podemos entender isso como uma espécie <i>check point</i>. Para salvar essa versão especifica vamos utilizar o conceito de <code>tag</code>. Essa <code>tag</code> demarcará um commit específico. Portanto após fazer um determinado commit que entenda-se como uma versão, release ou ponto importante do projeto demarcaremos a mesma com uma <code>tag</code>. Vejamos o exemplo:
</p>

```bash
$ git tag -a <aqui_minha_versão> -m <"aqui minha mensagem">
```
<p align = "justify">
  Caso o projeto já tenha registrado alguma <i>tag</i> a mesma poderá ser consultada através do seguinte comando:
</p>

```bash
$ git tag
```
```bash
2023.2
2023.3
2023.4
```

<p align = "justify">
  Você também pode consultar com mais detalhes cada uma das <i>tags</i> do projeto usando o seguinte comando:
</p>

```bash
$ git show <tag desejada>
```
```bash
commit c85a8a69876ba6bb55a4747189ac84975e9b41eb (tag: 2023.2)
Author: wmpjrufg <wanderlei_junior@ufcat.edu.br>
Date:   Sat May 27 22:19:31 2023 -0300
```
{: .note} 
> Aqui você poderá consultar informações como data, quem foi o usuário que realizou a modificação e até mesmo os detalhes do commit realizado a época.

<p align = "justify">
  Da mesma forma que <i>branchs</i> as <i>tags</i> também podem ser deletadas nas máquinas locais e no repositório remoto com os seguintes comandos: 
</p>

```bash
$ git tag -d <versão_que_deseja_deletar> # Deletando localmente
$ git push --delete origin <versão_que_deseja_deletar> # Deletando localmente
```

<p align = "justify">
  Por exemplo poderiamos deletar a versão <code>2023.2</code> no nosso exemplo com o seguinte comando. 
</p>

```bash
$ git tag -d 2023.2
$ git push --delete origin 2023.2
```

<p align = "justify">
  Para publicar uma tag então basta empregar o seguinte comando:
</p>

```bash
$ git push origin <versão_que_deseja_publicar>
```
{: .note} 
> Se for empregado o comando `git log` você poderá perceber que o último commit realizado antes da atribuição da _tag_ terá uma nova demaração. Vejamos o exemplo de um commit que foi atribuida uma _tag_: `commit 04da5f201fe9e01950a8b943e3911e6861c62137 (HEAD -> main, tag: 2023.4.3, origin/main, origin/HEAD)`.
