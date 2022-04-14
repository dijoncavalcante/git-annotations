# git-annotations
Annotations to help daily

## git fetch
Downloads das branches do servidor

## git cherry-pick [colocar-sha1-do-commit]
fazer cherry-pick de uma branch pra outra, estando na branch que vai receber

## git reset --hard HEAD@{44}
voltando pra uma branch especifica

## git reflog
vendo o que aconteceu na branch:

## git log --oneline
visualizar logs por linha:

## git reset --soft HEAD~1

## git reset --hard HEAD~1
voltar 1 commit
git push -f

## git rebase -i
git rebase -i HEAD~2                   <br/>
p de pick   -> no commit principal     <br/>
s de squash -> nos commits restantes   <br/>
Control + c -> quando terminar a edição<br/>
:x + enter                             <br/>
git push -f origin branch              <br/>

# Como unir meus commit em 1 único commit usando rebase
após o HEAD~ voce add a quantidade de commits que você quer usar <br/>
<b>  git rebase -i HEAD~2  <b> <br/>
no unix, você deve escolher o commit principal usando o p de pick e nos commit posteriores s de squash <br/>
para sair e salvar você usa <br/>
<b>  :x + enter  <b/>   <br/>
por ultimo voce faz o push <br/>
<b>  git push -f origin branch  <b/>  


## git restore --staged <file>
voltar arquivos no staged
  
## git diff
visualizar mudanças
  
## git branch -D branch
deletar branch local
  
## git branch -m novo-nome
rename ou renomear branch local

## git reset --hard origin/branch
resetar modificações de uma branch, apenas criar uma outra branch e executar esse comando


## steps	git rebase
git pull --rebase origin branch            <br/>
Resolver conflitos e marcar como RESOLVIDO <br/>
git status                                 <br/>
git rebase --continue                      <br/>
Aparece o UNIX                             <br/>
Digitar :w                                 <br/>
Digitar :q                                 <br/>
Rebuild                                    <br/>
git push -f origin branch                  <br/>
