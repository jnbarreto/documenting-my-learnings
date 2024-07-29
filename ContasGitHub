***COMANDOS PARA TRABALHAR COM O GIT COM 2 CONTAS***

cd ~
touch .gitconfig .gitconfig-personal .gitconfig-work


vim .gitconfig

------------------------------------ arquivo 
[user]
	name = Juan Barreto
[includeIf "gitdir:~/.workspace/personal/"]
	path = ~/.gitconfig-personal
[includeIf "gitdir:~/.workspace/work/"]
	path = ~/.gitconfig-work

--------------------------------------------
vim .gitconfig-personal

-------------------------------------------- arquivo 
[user]
	name = Juan Carlos Leone Barreto
	email = jc.leone98@gmail.com
[core]
	sshCommand = "ssh -i ~/.ssh/personal_id_rsa"

---------------------------------------------------

vim .gitconfig-work

-------------------------------------------- arquivo 
[user]
	name = Juan Carlos Leone Barreto
	email = juan.carlos@codee.tech
[core]
	sshCommand = "ssh -i ~/.ssh/work_id_rsa"

----------------------------------------------------	

cd ~
mkdir workspace
cd workspace
mkdir personal work

***CRIANDO AS CHAVES SSH ***
cd ~/.ssh
ssh-keygen -f personal_id_rsa
ssh-keygen -f work_id_rsa

***COPIE AS CHAVES SSH PARA SEUS RESPECTIVOS REPOSITORIOS***
cd ~/.ssh
cat personal_id_rsa.pub
cat work_id_rsa.pub






