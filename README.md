# cursoJsUser

#treinando uso do Java Script
#versionado entre PC e Not afim de aprender mais sobre o git e seus comandos

$ git remote -v
$ git remote rm origin
$ git commit -m "your commit"
$ git remote add origin https://github.com/user/repo.git
$ git push -f origin master
git remote add origin git@github.com:felipe-f-dantas/app2.git

erro: abaixo

To github.com:felipe-f-dantas/app2.git
! [rejected] master -> master (non-fast-forward)
error: failed to push some refs to 'git@github.com:felipe-f-dantas/app2.git'
hint: Updates were rejected because the tip of your current branch is behind
hint: its remote counterpart. Integrate the remote changes (e.g.
hint: 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.

Lidar com erros non-fast-forward
Às vezes, o Git não pode fazer sua alteração em um repositório remote sem perder os commits. Quando isso acontece, seu push é recusado.

Se outra pessoa tiver feito push no mesmo branch que você, o Git não poderá fazer push das alterações:

$ git push origin main

> To https://github.com/USERNAME/REPOSITORY.git
> ! [rejected] main -> main (non-fast-forward)
> error: failed to push some refs to 'https://github.com/USERNAME/REPOSITORY.git'
> To prevent you from losing history, non-fast-forward updates were rejected
> Merge the remote changes (e.g. 'git pull') before pushing again. See the
> 'Note about fast-forwards' section of 'git push --help' for details.
> Você pode corrigir isso fazendo fetch e merge das alterações feitas no branch remote com as alterações que foram feitas localmente:

$ git fetch origin

# Faz fetch das atualizações feitas em um repositório online

$ git merge origin YOUR_BRANCH_NAME

# Faz merge de atualizações feitas online com seu trabalho local

git push -f origin master // forca o envio dos arquivos

echo "# cara_ou_coroa" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M master
git remote add origin https://github.com/felipe-f-dantas/cara_ou_coroa.git
git push -u origin master
…or push an existing repository from the command line
git remote add origin https://github.com/felipe-f-dantas/cara_ou_coroa.git
git branch -M master
git push -u origin master

problemas com remote: No anonymous write access.
fatal: Authentication failed for .... Ajuda abaixo

https://stackoverflow.com/questions/60757334/git-push-from-visual-studio-code-no-anonymous-write-access-authentication-fai
