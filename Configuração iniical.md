## Configuração

### Geral

As configurações do GIT são armazenadas no arquivo **.gitconfig** localizado dentro do diretório do usuário do Sistema Operacional (Ex.: Windows: C:\Users\Documents and Settings\Leonardo ou *nix /home/leonardo).
As configurações realizadas através dos comandos abaixo serão incluídas no arquivo citado acima.
##### Setar usuário
	git config --global user.name "Evandro Moreira"
##### Setar email
	git config --global user.email "evandroarlati@hotmail.com"	
##### Setar editor
	git config --global core.editor vim
##### Verificar configurações individual
	git config user.name
	git config user.email	
	git config core.editor
  ##### Verificar todas as configurações
	git config --list
  
