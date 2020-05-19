# GIT E GITHUB

Guia prático para iniciantes.

### Instalação

https://git-scm.com/downloads

# SCENES

- [x] Você deseja criar pontos na história da produção do seu projeto.
    - git init (iniciar repositório onde será guardado as alterações do projeto)
    - git add ARQUIVO (adiciona um ponto na história)
    - git commit -m "first commit" (leva o ponto criado até o repositório)
- [x] Você deseja verificar mudanças feitas no seu projeto.
    - git log (mostra todos os pontos criados)
    - git status (mostra o status das alterações do projeto)
    - git show (mostra o último ponto na história)
    - git show IDDOCOMMIT (mostra um ponto específico)

- [x] Você começa uma nova funcionalidade no seu projeto, sem estragar o que foi feito.
    - git branch (mostra todas as ramificações)
    - git branch NOMEDABRANCH (cria uma nova ramificação)
    - git checkout NOMEDABRANCH (alterna entre as ramificações)
    - git checkout -b NOMEDABRANCH (cria e alterna para a nova ramificação)
- [x] Você adiciona as novas funcionalidades ao seu projeto em produção.
    - git merge NOMEDABRANCH (une duas ramificações em uma)
- [x] Você quer deletar a branch da nova funcionalidade, depois de aplicar em seu projeto.
    - git branch -D NOMEDABRANCH (deleta uma ramificação)

- [x] Colocar o projeto na nuvem.
    - git push -u origin master URLDOREPOSITORIOREMOTO (envia o projeto para um repositório remoto e cria a ramificação master)
    - git config credential.helper store (armazena as credencias do repositório remoto)
    - git remove -v (mostra todos os repositórios remotos)

- [x] Você vai pegar um projeto já iniciado, para trabalhar com o time.
    - git clone URLDOREPOSITORIOREMOTO (clona um repositório remoto para a máquina local)
- [x] Você precisa resolver um conflito.
    - git checkout -b test
    - nano arquivo.html
    - git commit -am "update arquivo.html"
    - git checkout master
    - nano arquivo.html
    - git add .
    - git commit -m "arquivo.html"
    - git merge test
    - git commit -am "conflict fixed"
- [x] Antes de enviar a resolução, precisamos atualizar o projeto local.
    - git pull (atuliza o repositório local com o remoto)

- [x] Você precisa voltar um arquivo para um determinado momento da linha do tempo.
    - git log
    - git checkout IDDOCOMMIT -- arquivo.html
    - git commit -am "restore arquivo.html"
- [x] Você precisa recuperar algo deletado.
    - rm lesson1/arquivo.html
    - git commit -am "delete arquivo.html"
    - git log
    - git checkout IDDOCOMMIT -- arquivo.html
