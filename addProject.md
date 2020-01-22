Adicionar um projeto existente ao GitHub usando a linha de comando

GitHub.com Importing your projects Importar código-fonte para o GitHub Adicionar um projeto existente ao GitHub usando a linha de comando
Adicionar um projeto existente ao GitHub usando a linha de comando
Colocar um trabalho que já existe no GitHub pode permitir que você compartilhe e colabore de muitas maneiras.

Mac
Windows
Linux
If you are migrating your project from CodePlex, read the migration guide for more information.

Dica: se estiver mais familiarizado com uma interface de usuário de apontar e clicar, tente adicionar seu projeto com o GitHub Desktop. Para obter mais informações, consulte "Adicionar um repositório do seu computador local ao GitHub Desktop" na Ajuda do GitHub Desktop.

Warning: Never git add, commit, or push sensitive information to a remote repository. Sensitive information can include, but is not limited to:

Passwords
Chaves SSH
AWS access keys
API keys
Credit card numbers
PIN numbers
Para obter mais informações, consulte "Remover dados confidenciais do repositório".

Crie um repositório no GitHub. Para evitar erros, não inicialize o novo repositório com os arquivos LEIAME, de licença ou gitignore. É possível adicionar esses arquivos após push do projeto no GitHub.

Menu suspenso Create New Repository (Criar novo repositório)
Open Git Bash.

Altere o diretório de trabalho atual para seu projeto local.

Inicialize o diretório local como um repositório Git.

$ git init
Adicione os arquivos ao novo repositório local. Isso faz stage deles para o primeiro commit.

$ git add .
# Adiciona os arquivos no repositório local e faz stage deles para commit. Para remover o stage de um arquivo, use "git reset HEAD YOUR-FILE".
Faça commit dos arquivos com stage em seu repositório local.

$ git commit -m "First commit"
# Faz commit das alterações controladas e as prepara para o push em um repositório remote. Para remover esse commit e modificar o arquivo, use "git reset --soft HEAD~1", faça o commit e adicione o arquivo novamente.
Na parte superior da página Quick Setup (Configuração rápida) do repositório do GitHub, clique em  para copiar a URL do repositório remote.

Campo Copy remote repository URL (Copiar URL do repositório remote)
No prompt de comando, adicione a URL para o repositório remote onde será feito push do seu repositório local.

$ git remote add origin remote repository URL
# Define o novo remote
$ git remote -v
# Verifica a nova URL remota
Faça push das alterações no seu repositório local para o GitHub.

$ git push -u origin master
# Faz push das alterações no seu repositório local até o repositório remote 
