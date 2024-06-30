<h1>Jogo do número secreto</h1>

<h2>🔖 Sobre</h2>
<p>Projeto utilizado nos cursos de lógica de programação da Alura.</p>

## 🚀 Tecnologias

<div>
  <img src="https://img.shields.io/badge/HTML-239120?style=for-the-badge&logo=html5&logoColor=white">
  <img src="https://img.shields.io/badge/CSS-239120?&style=for-the-badge&logo=css3&logoColor=white">
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black">
</div>

# Time

| [<img loading="lazy" src="https://avatars.githubusercontent.com/u/33001620?v=4" width=115><br><sub>Gabrielle Ribeiro</sub>](https://github.com/gabrielle-ribeiro) | [<img loading="lazy" src="https://avatars.githubusercontent.com/u/522931?v=4" width=115><br><sub>Rodrigo Caneppele</sub>](https://github.com/rcaneppele) |
| :---------------------------------------------------------------------------------------------------------------------------------------------------------------: | :------------------------------------------------------------------------------------------------------------------------------------------------------: |

-- Configurar nome de usuário e email
-- git config --global user.name "Seu Nome": define o nome de usuário global
-- git config --global user.email "seu.email@example.com": define o email global

-- Criar um novo repositório
-- git init: inicializa um novo repositório Git na pasta atual

-- Clonar um repositório existente
-- git clone <url-do-repositorio>: faz uma cópia de um repositório remoto para a sua máquina

-- Verificar o status dos arquivos
-- git status: mostra o status das mudanças no repositório

-- Adicionar arquivos para a área de stage
-- git add <nome-do-arquivo>: adiciona um arquivo específico para a área de stage
-- git add .: adiciona todos os arquivos modificados para a área de stage

-- Fazer commit das alterações
-- git commit -m "Mensagem descritiva do commit": grava as mudanças adicionadas na área de stage

-- Visualizar o histórico de commits
-- git log: exibe o histórico de commits do repositório

-- Criar uma nova branch
-- git branch <nome-da-branch>: cria uma nova branch no repositório
-- Observação: Uma branch (ramificação) é uma linha separada de desenvolvimento. Você pode usar branches para trabalhar em diferentes funcionalidades ou correções de bugs de forma isolada.

-- Mudar para outra branch
-- git checkout <nome-da-branch>: muda para a branch especificada

-- Criar e mudar para uma nova branch
-- git checkout -b <nome-da-branch>: cria uma nova branch e muda para ela imediatamente

-- Mesclar uma branch com a branch atual
-- git merge <nome-da-branch>: mescla a branch especificada com a branch atual
-- Observação: O merge (mesclagem) combina mudanças de diferentes branches. Isso é útil para integrar funcionalidades ou correções de bugs desenvolvidas separadamente.

-- Remover uma branch local
-- git branch -d <nome-da-branch>: remove a branch especificada localmente

-- Enviar uma branch para o repositório remoto
-- git push origin <nome-da-branch>: envia a branch especificada para o repositório remoto

-- Remover uma branch do repositório remoto
-- git push origin --delete <nome-da-branch>: remove a branch especificada do repositório remoto

-- Verificar repositórios remotos
-- git remote -v: exibe os repositórios remotos configurados

-- Adicionar um repositório remoto
-- git remote add origin <url-do-repositorio>: adiciona um novo repositório remoto com o nome "origin"

-- Enviar commits para o repositório remoto
-- git push origin <nome-da-branch>: envia os commits da branch especificada para o repositório remoto

-- Atualizar o repositório local com mudanças do remoto
-- git pull origin <nome-da-branch>: puxa as mudanças da branch especificada no repositório remoto para o repositório local

-- Reverter mudanças locais
-- git checkout -- <nome-do-arquivo>: desfaz mudanças não comitadas em um arquivo específico

-- Desfazer um commit específico (mantendo mudanças)
-- git reset --soft <id-do-commit>: desfaz o commit especificado, mantendo as mudanças na área de stage

-- Desfazer um commit específico (descartando mudanças)
-- git reset --hard <id-do-commit>: desfaz o commit especificado e descarta todas as mudanças

Restorar para o último commit
-- git restore . --> restaura tudo
-- git checkout -- . --> mesma coisa

restaura pra o último commit.
git restore --staged app.js

Tags: Pontos específicos no código
git tag <nome> ou <id> ponteiro para algum commit específico.
git push origin --<nome da tag> ou sem especificar
git tag -d <nome> -- remove a tag
git tag -a <nome> -m <mensagem>
git tag -v <nome> --> mostra as informações

Releases -- nome da tag

Reaproveitando commits de uma branch em outros cenários
faço o git logo com o nome da branch específica
git cherry-pick <hash do commit>

Achar o culpado, não acho que isso é uma boa ideia:
git blame <arquivo>

-- Comandos do gitgub acima do básico
-- git log: mostra os commuts e informações
-- git log --oneline -- mostra informações resumidas
-- git log -p -- exibe mais informações
-- git log --graph
-- git log --format="%H %an"

-- git diff --> visualiza os estados atuais e o último commit.

git diff commitatingo..commitNovo --> verifica as diferenças
