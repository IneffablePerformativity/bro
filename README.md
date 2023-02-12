# bro
Let bro and sis be peers in repo folder, but sis a submodule of bro.

Yet another failure:

:~$ cd ~/repo
:~/repo$ rm -rf *
:~/repo$ git clone git@github.com:IneffablePerformativity/bro.git
Cloning into 'bro'...
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Compressing objects: 100% (2/2), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
Receiving objects: 100% (3/3), done.
:~/repo$ cd bro
:~/repo/bro$ git submodule add git@github.com:IneffablePerformativity/sis.git ../sis
fatal: ../sis: '../sis' is outside repository at '/home/ajs/repo/bro'

