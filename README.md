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


# DOTNET CLI #

## Definitions ##

Defined commands by .net

-  dotnet --version

​		verify actual version

-  dotnet --list-runtimes

  List installed SDKs

- dotnet --list-runtimes

  List installed runtimes

- dotnet help

  Show Help

  List Commands

## New Project ##

## dotnet CLI definitions ##

- dotnet new console
- dotnet new classlib
- dotnet new mvc
- dotnet new webapi
- dotnet new mstest

## dotnet packages installation

[string] packList = [
   Microsoft.AspNetCore.Mvc           2.2.0       2.2.0   
   EntityFrameworkCore.Design         7.0.2       7.0.2   
   EntityFrameworkCore.SqlServer      7.0.2       7.0.2   
   Newtonsoft.Json                    13.0.2      13.0.2  
];

dotnet add package $"Microsoft.{packList}"

## # float# (32-bits)

- 3.402823e38 at 3.402823e38

## ** double (64-bit) ** 

- -1.79769313486232e308 at 1.79769313486232e308

## @ **decimal (128-bit) ** @

- +-1.0 x 10e-28 at 7.9 x 10e29


## Docker Sql Server Installation

sudo docker run -e "ACCEPT_EULA=Y" -e "MSSQL_SA_PASSWORD=<?php$mssql?>" \
    -p 1433:1433 --name sql1 --hostname sql1 \
    -d \
    mcr.microsoft.com/mssql/server:2022-latest
#### Completed command change: sql2 version
docker run -e "ACCEPT_EULA=Y" -e "SA_PASSWORD=<?php$mssql>" \
    -v /db/:/var/opt/mssql/data \
    -p 1433:1433  \
    --rm --name sql2 \
    -h sql1 \
    -d mcr.microsoft.com/mssql/server:2019-latest \
    --restart=always 

sudo docker exec -it sql2 /opt/mssql-tools/bin/sqlcmd \
    -S localhost -U SA \
    -P "$(read -sp "Enter current SA password: "; echo "${REPLY}")" \
    -Q "ALTER LOGIN SA WITH PASSWORD=\"$(read -sp "Enter new SA password: "; echo "${REPLY}")\""

docker run -d -v $(pwd)/db:/opt/ -p 1433:1433 --rm --name sql2 mcr.microsoft.com/mssql/server

          sudo docker exec -it sql2 "bash"









