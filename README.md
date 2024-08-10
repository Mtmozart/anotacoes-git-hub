<h1>Jogo do número secreto</h1>

<h2>🔖 Sobre</h2>
<p>Projeto utilizado nos cursos de lógica de programação da Alura.</p>

Aqui está o conteúdo formatado com anotações para melhor legibilidade:

## 🚀 Tecnologias

<div>
  <img src="https://img.shields.io/badge/HTML-239120?style=for-the-badge&logo=html5&logoColor=white">
  <img src="https://img.shields.io/badge/CSS-239120?&style=for-the-badge&logo=css3&logoColor=white">
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black">
</div>

# Criado pela Alura

## Configurações Básicas

- **Configurar nome de usuário e email:**
  - `git config --global user.name "Seu Nome"`: define o nome de usuário global.
  - `git config --global user.email "seu.email@example.com"`: define o email global.

## Comandos Básicos de Git

- **Criar um novo repositório:**
  - `git init`: inicializa um novo repositório Git na pasta atual.

- **Clonar um repositório existente:**
  - `git clone <url-do-repositorio>`: faz uma cópia de um repositório remoto para a sua máquina.

- **Verificar o status dos arquivos:**
  - `git status`: mostra o status das mudanças no repositório.

- **Adicionar arquivos para a área de stage:**
  - `git add <nome-do-arquivo>`: adiciona um arquivo específico para a área de stage.
  - `git add .`: adiciona todos os arquivos modificados para a área de stage.

- **Fazer commit das alterações:**
  - `git commit -m "Mensagem descritiva do commit"`: grava as mudanças adicionadas na área de stage.

- **Visualizar o histórico de commits:**
  - `git log`: exibe o histórico de commits do repositório.

## Trabalhando com Branches

- **Criar uma nova branch:**
  - `git branch <nome-da-branch>`: cria uma nova branch no repositório.

- **Mudar para outra branch:**
  - `git checkout <nome-da-branch>`: muda para a branch especificada.

- **Criar e mudar para uma nova branch:**
  - `git checkout -b <nome-da-branch>`: cria uma nova branch e muda para ela imediatamente.

- **Mesclar uma branch com a branch atual:**
  - `git merge <nome-da-branch>`: mescla a branch especificada com a branch atual.

- **Remover uma branch local:**
  - `git branch -d <nome-da-branch>`: remove a branch especificada localmente.

## Interagindo com Repositórios Remotos

- **Enviar uma branch para o repositório remoto:**
  - `git push origin <nome-da-branch>`: envia a branch especificada para o repositório remoto.

- **Remover uma branch do repositório remoto:**
  - `git push origin --delete <nome-da-branch>`: remove a branch especificada do repositório remoto.

- **Verificar repositórios remotos:**
  - `git remote -v`: exibe os repositórios remotos configurados.

- **Adicionar um repositório remoto:**
  - `git remote add origin <url-do-repositorio>`: adiciona um novo repositório remoto com o nome "origin".

- **Enviar commits para o repositório remoto:**
  - `git push origin <nome-da-branch>`: envia os commits da branch especificada para o repositório remoto.

- **Atualizar o repositório local com mudanças do remoto:**
  - `git pull origin <nome-da-branch>`: puxa as mudanças da branch especificada no repositório remoto para o repositório local.

## Revertendo e Restaurando Alterações

- **Reverter mudanças locais:**
  - `git checkout -- <nome-do-arquivo>`: desfaz mudanças não comitadas em um arquivo específico.

- **Desfazer um commit específico mantendo as mudanças:**
  - `git reset --soft <id-do-commit>`: desfaz o commit especificado, mantendo as mudanças na área de stage.

- **Desfazer um commit específico descartando as mudanças:**
  - `git reset --hard <id-do-commit>`: desfaz o commit especificado e descarta todas as mudanças.

- **Restaurar para o último commit:**
  - `git restore .`: restaura tudo.
  - `git checkout -- .`: mesma coisa.
  - `git restore --staged app.js`: restaura um arquivo específico da área de stage.

## Trabalhando com Tags

- **Criar e gerenciar tags:**
  - `git tag <nome>`: cria uma tag.
  - `git push origin --<nome da tag>`: envia a tag para o repositório remoto.
  - `git tag -d <nome>`: remove a tag localmente.
  - `git tag -a <nome> -m <mensagem>`: cria uma tag anotada com uma mensagem.
  - `git tag -v <nome>`: exibe informações sobre a tag.

## Utilizando Commits em Outros Cenários

- **Reaproveitar commits de uma branch:**
  - `git cherry-pick <hash do commit>`: aplica um commit específico de outra branch na branch atual.

## Comandos Avançados

- **Verificar o autor das alterações (git blame):**
  - `git blame <arquivo>`: mostra o autor de cada linha de um arquivo, mas pode não ser a melhor prática.

- **Comandos avançados de log:**
  - `git log`: mostra os commits e informações detalhadas.
  - `git log --oneline`: mostra informações resumidas.
  - `git log -p`: exibe mais informações detalhadas.
  - `git log --graph`: exibe um gráfico dos commits.
  - `git log --format="%H %an"`: formata a saída do log com hash e autor.

- **Visualizar diferenças entre commits:**
  - `git diff`: visualiza as diferenças entre o estado atual e o último commit.
  - `git diff <commitAntigo>..<commitNovo>`: verifica as diferenças entre dois commits específicos.

Essa estrutura com anotações facilita o entendimento e a navegação pelos comandos do Git.
