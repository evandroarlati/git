## Configuração

### Geral

As configurações do GIT são armazenadas no arquivo **.gitconfig** localizado dentro do diretório do usuário do Sistema Operacional (Ex.: Windows: C:\Users\Documents and Settings\Leonardo ou *nix /home/leonardo).
As configurações realizadas através dos comandos abaixo serão incluídas no arquivo citado acima.
##### Setar usuário
	git config --global user.name "Evandro Moreira"
##### Setar email
	git config --global user.email "evandroarlati@hotmail.com"	
##### Setar editor
	git config --global core.editor "code --wait"
##### Verificar configurações individual
	git config user.name
	git config user.email	
	git config core.editor
  ##### Verificar todas as configurações
	git config --list
  


## Conectando ao GitHub com SSH

Mais detalhes em  [Connecting to GitHub with SSH](https://help.github.com/en/github/authenticating-to-github/connecting-to-github-with-ssh)

### Generating a new SSH key
1. Open Git Bash.

2. Paste the text below, substituting in your GitHub email address.

$ ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
This creates a new ssh key, using the provided email as a label.

> Generating public/private rsa key pair.
When you're prompted to "Enter a file in which to save the key," press Enter. This accepts the default file location.

> Enter a file in which to save the key (/c/Users/you/.ssh/id_rsa):[Press enter]
At the prompt, type a secure passphrase. For more information, see "Working with SSH key passphrases".

> Enter passphrase (empty for no passphrase): [Type a passphrase]
>