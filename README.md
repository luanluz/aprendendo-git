# GIT E GITHUB

Guia prático para iniciantes.

### Instalação

https://git-scm.com/downloads

# SCENES

- [x] Você deseja criar pontos na história da produção do seu projeto.
    - git init _iniciar repositório onde será guardado as alterações do projeto_
    - git add ARQUIVO _adiciona um ponto na história_
    - git commit -m "first commit" _leva o ponto criado até o repositório_
- [x] Você deseja verificar mudanças feitas no seu projeto.
    - git log _mostra todos os pontos criados_
    - git status _mostra o status das alterações do projeto_
    - git show _mostra o último ponto na história_
    - git show IDDOCOMMIT _mostra um ponto específico_

- [x] Você começa uma nova funcionalidade no seu projeto, sem estragar o que foi feito.
    - git branch _mostra todas as ramificações_
    - git branch NOMEDABRANCH _cria uma nova ramificação_
    - git checkout NOMEDABRANCH _alterna entre as ramificações_
    - git checkout -b NOMEDABRANCH _cria e alterna para a nova ramificação_
- [x] Você adiciona as novas funcionalidades ao seu projeto em produção.
    - git merge NOMEDABRANCH _une duas ramificações em uma_
- [x] Você quer deletar a branch da nova funcionalidade, depois de aplicar em seu projeto.
    - git branch -D NOMEDABRANCH _deleta uma ramificação_

- [x] Colocar o projeto na nuvem.
    - git push -u origin master URLDOREPOSITORIOREMOTO _envia o projeto para um repositório remoto e cria a ramificação master_
    - git config credential.helper store _armazena as credencias do repositório remoto_
    - git remove -v _mostra todos os repositórios remotos_

- [x] Você vai pegar um projeto já iniciado, para trabalhar com o time.
    - git clone URLDOREPOSITORIOREMOTO _clona um repositório remoto para a máquina local_
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
    - git pull _atuliza o repositório local com o remoto_

- [x] Você precisa voltar um arquivo para um determinado momento da linha do tempo.
    - git log
    - git checkout IDDOCOMMIT -- arquivo.html
    - git commit -am "restore arquivo.html"
- [x] Você precisa recuperar algo deletado.
    - rm lesson1/arquivo.html
    - git commit -am "delete arquivo.html"
    - git log
    - git checkout IDDOCOMMIT -- arquivo.html
