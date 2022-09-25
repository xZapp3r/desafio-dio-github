# desafio-dio-github
Neste desafio estamos. Desafio de Projeto sobre Git\Github


code -r . >(in a repo to open in code)

git status >(see commits and branches)

git log >( history of the current branches branches )

git checkout -b testing-demo  >(create a new branche) <--CREATE-->

git branch  >(shows the branches that you have ) 

git status >(in the next could select the files that you want to upload ) and ( show the modified files )

git add {file-name.pgp} >( put the file on a staged before putting on commit in github )

git commit -m 'testin out' >( put some description and commit the staged files on the local repository )

git remote -v >( shows the remote repositories options )

gir remote add upstream git@github.com:{profile=xZapper}/{project=Spotify-Clone} >(pull the remote upstr branche )

git fetch {upstream} >(update your local repository with the upstream)

>*TO pull to master the heads need to be equal == null*

git reset >(made the branch null to be pulled )

git checkout master >(go to the master branch and verify syncronous files )

git reset --hard master/upstream >( force matching branches )

git push origin master >(pull a request to be commited )

git push upstream master >(push directly to the master branche ) << Need permission >>









