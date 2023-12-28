---
layout: default
title: Guardando versão
nav_order: 6
parent: Git e GitHub na prática
---

<p align = "justify">
  Na plataforma git hub é possível registrar ou especificar pontos do algoritmo que achamos importantes, podemos entender isso como uma espécie <i>check point</i>. Para salvar essa versão especifica vamos utilizar as <code>tags</tags>. 
</p>

```bash
$ git revert código_hash_do_commit
```
<p>
Reverte o Commit através do ID de identificação.

{: .note} 
>Pode-se dizer que este comando é um <i>commit</i>, porém ele realiza o efeito inverso do <a href = "https://wmpjrufg.github.io/GIT0001/002-2.html#commit"><i>git commit</i></a>.

</p>

```bash
$ git revert head
```
<p>
Reverte o último Commit feito.
</p>

<p>
Acesse <a href = "https://git-scm.com/docs/git-revert/pt_BR">aqui</a> a documentação completa.
</p>
