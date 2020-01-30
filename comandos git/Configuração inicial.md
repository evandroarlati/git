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


Adding a new SSH key to your GitHub account
To configure your GitHub account to use your new (or existing) SSH key, you'll also need to add it to your GitHub account.

Mac
Windows
Linux
Before adding a new SSH key to your GitHub account, you should have:

Checked for existing SSH keys
Generated a new SSH key and added it to the ssh-agent
After adding a new SSH key to your GitHub account, you can reconfigure any local repositories to use SSH. For more information, see "Switching remote URLs from HTTPS to SSH."

Note: DSA keys (SSH-DSS) are no longer supported. Existing keys will continue to function, but you cannot add new DSA keys to your GitHub account.

Copy the SSH key to your clipboard.

If your SSH key file has a different name than the example code, modify the filename to match your current setup. When copying your key, don't add any newlines or whitespace.

$ clip < ~/.ssh/id_rsa.pub
# Copies the contents of the id_rsa.pub file to your clipboard
Tip: If clip isn't working, you can locate the hidden .ssh folder, open the file in your favorite text editor, and copy it to your clipboard.

In the upper-right corner of any page, click your profile photo, then click Settings.

Settings icon in the user bar
In the user settings sidebar, click SSH and GPG keys.

Authentication keys
Click New SSH key or Add SSH key.

SSH Key button
In the "Title" field, add a descriptive label for the new key. For example, if you're using a personal Mac, you might call this key "Personal MacBook Air".

Paste your key into the "Key" field.

The key field
Click Add SSH key.

The Add key button
If prompted, confirm your GitHub password.

Sudo mode dialog