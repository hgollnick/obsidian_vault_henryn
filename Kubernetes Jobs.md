[[Kubernetes]]

echo -n '<secret>' | base64

1) Authenticate to Kubernetes Cluster

                [https://dwoeacp-api.dewoe.corpintra.net:32001](https://dwoeacp-api.dewoe.corpintra.net:32001)

                [https://iwoeacp-api.dewoe.corpintra.net:32001](https://iwoeacp-api.dewoe.corpintra.net:32001)

                [https://swoeacp-api.dewoe.corpintra.net:32001](https://swoeacp-api.dewoe.corpintra.net:32001)

                [https://swoeacp-api.dewoe.corpintra.net:32001/commandline](https://swoeacp-api.dewoe.corpintra.net:32001/commandline)

echo -n 'svI_Hm)uzKacJKZOvzcE' | base64 c3ZJX0htKXV6S2FjSktaT3Z6Y0U=

kubectl get secret -n a4t-wspdoku wspdoku-cronjob-secret --template={{.data.cft_pw}}

# List the Secret names

kubectl get secrets -n a4t-wspdoku

# Show the Secret content. example: oidcClientSecret

kubectl get secret -n a4t-wspdoku wspdoku-alaea-simulation-cronjob-secret --template={{.data.alaea_simulation.db_pw}}

alaea_simulation.db_pw

wspdoku-alaea-simulation-cronjob-secret.yaml

**************************************************************

kubectl commands

**************************************************************

$ kubectl version  

$ kubectl api-versions

$ kubectl --help

$ ./dev-deploy.sh delete sca

$ ./dev-deploy.sh apply sca

kubectl get pods -n a4t-sca

$ kubectl get jobs -n a4t-sca

kubectl get pods -n a4t-wspdoku

$ kubectl describe pods -n a4t-wspdoku

$ kubectl describe pod sca-deployment-575869fbdc-z9grl -n a4t-sca

$ kubectl describe pod ascot-cronjob-ftp-download-as400-1632397800-mqb6x -n a4t-ascot

$ kubectl describe pod wspdoku-deployment-6d5b499d96-hgvfk -n a4t-wspdoku

$ kubectl describe jobs -n a4t-wspdoku -f wspdoku-epdmu-export-bcs-d-cronjob-1629285900-fzpnp

$ kubectl get cj -n a4t-sca

$ kubectl get cj -n a4t-wspdoku

$ kubectl get cj -n a4t-sca -o yaml

$ kubectl get cj wspdoku-cronjob-epdmu-import  -n a4t-sca -o yaml

$ kubectl create -f sca-cronjob-mv-files.yaml

$ kubectl delete -f sca-cronjob-mv-files.yaml

$ kubectl create -f sca-cronjob-ftp-download-as400.yaml

$ kubectl delete -f sca-cronjob-ftp-download-as400.yaml

$ kubectl delete -f sca-cronjob-cp-files-config-map.yaml

$ kubectl apply -f sca-cronjob-mv-files-config-map.yaml

$ kubectl apply -f sca-cronjob-ftp-download-as400-config-map.yaml

$ kubectl apply -f ascot-cronjob-ftp-download-as400-config-map.yaml

$ kubectl get cm -n a4t-sca

$ kubectl get cm sca-cronjob-mv-files-config-map -o yaml -n a4t-sca

$ kubectl get cm sca-cronjob-ftp-download-as400-config-map -o yaml -n a4t-sca

$ kubectl apply -f wspdoku-promos-exporter-cronjob.yaml

$ kubectl delete -f wspdoku-promos-exporter-cronjob.yaml

$ kubectl apply -f wspdoku-promos-exporter-cronjob-config-map.yaml

$ kubectl delete -f wspdoku-cronjob-epdmu-import.yaml

$ kubectl get cj wspdoku-promos-exporter-cronjob -n a4t-wspdoku -o yaml

$ kubectl apply -f sca-cronjob-mv-files.yaml

$ kubectl apply -f sca-cronjob-ftp-download-as400.yaml 

$ kubectl apply -f ascot-cronjob-ftp-download-as400.yaml 

$ kubectl delete -f ascot-cronjob-ftp-download-as400.yaml 

$ kubectl describe pod ascot-cronjob-ftp-download-as400-1625889600-bndw8 -n a4t-ascot

$ kubectl describe pod wspdoku-promos-bba-cronjob-1652946000-z9h6r -n a4t-wspdoku

$ kubectl apply -f sca-cronjob-secret.yaml

$ kubectl apply -f ascot-cronjob-secret.yaml

$ kubectl delete --all pods --namespace=a4t-wspdoku --force

kubectl delete pod --grace-period=0 --force --namespace a4t-ascot ascot-cronjob-ftp-download-as400-1626105600-7kcg6

kubectl delete pod --grace-period=0 --force --namespace a4t-wspdoku wspdoku-promos-exporter-cronjob-1628109600

ascot-cronjob-ftp-download-as400-1626105600-7kcg6

$ kubectl config use-context sca

kubectl logs -n a4t-wspdoku -f wspdoku-promos-bba-cronjob-1642082700-z9njh > /c/temp/amsys.dev.log

$ kubectl logs -n a4t-sca -f sca-cronjob-mv-files-1625092800-mn6pc 

To force delete all pods in a namesapce at once

ktl get pods -o custom-columns=:metadata.name | xargs kubectl delete pod --force --grace-period=0

sudo journalctl -u kubelet | grep "ascot-cronjob-ftp-download-as400-1625889600-bndw8"

wspdoku-promos-exporter-cronjob-1628110800-7z6q5

$ kubectl logs -n a4t-wspdoku -f wspdoku-promos-exporter-cronjob-1628113200-msffb > /c/temp/wspdoku-promos-exporter-cronjob-dev.log

$ kubectl get pod -n a4t-ascot -p ascot-cronjob-ftp-download-as400-1626105600-7kcg6 -o yaml > /c/temp/runbooks_pod_configuration.txt

$ kubectl get pod -n a4t-ascot -f ascot-cronjob-ftp-download-as400-1626105600-7kcg6 -o yaml > /c/temp/runbooks_pod_configuration.txt

$ kubectl get pod -n [NAMESPACE] -p [POD_NAME] -o yaml

**************************************************************

CREATE JOB

**************************************************************

--- change into sca for creating job !!!!

$ cd /c/work/repos/git/k8s-dev/sca

$ kubectl get jobs -n a4t-sca

$ kubectl describe jobs -n a4t-sca

-- CREATE JOB

$ kubectl create -f sca-cronjob-mv-files.yaml

cronjob.batch/sca-cronjob-cp created

$ kubectl apply -f sca-cronjob-mv-files.yaml

$ kubectl create -f sca-cronjob-test.yaml

--- DELETE JOB

$ kubectl delete -f sca-cronjob-cp.yaml

cronjob.batch "sca-cronjob-cp" deleted

$ kubectl delete -f sca-cronjob-cp-files.yaml

$ kubectl delete -f sca-cronjob-mv-files.yaml

Created pod: sca-cronjob-test-1622811300-vjbz7

sca-cronjob-cp-1623327300

pods=$(kubectl get pods --selector=job-name=sca-cronjob-test-1623328500 --output=jsonpath='{.items[*].metadata.name}')

echo $pods

sca-cronjob-test-1623328740-p6wx5

$ kubectl logs -n a4t-sca -f sca-cronjob-mv-files-1624883400-x2jgj    > /c/temp/a4t-sca-cronjob.dev.log

sca-cronjob-mv-files-1624881600-x5cth

$ kubectl logs -n a4t-sca -f sca-cronjob-test-1623327540 > /c/temp/a4t-sca-job.dev.log

./dev-deploy.sh delete sca

"kubectl delete --all pods -n a4t-sca" müsste das Einfachste sein. Dann ist aber auch der Application Pod weg

$ kubectl delete cronjob sca-cronjob-test

--- doesn work

$ kubectl get cronjob sca-cronjob-test

Error from server (Forbidden): cronjobs.batch "sca-cronjob-test" is forbidden: User [anita.ruegsegger@t-systems.com](mailto:anita.ruegsegger@t-systems.com) cannot get resource "cronjobs" in API grouespace "default"

# Replace "hello-4111706356" with the job name in your system

pods=$(kubectl get pods --selector=job-name=sca-cronjob-test-1622808840 --output=jsonpath={.items[*].metadata.name})

kubectl logs $pods

Erst mit kubectl get cronjob den Namen ermitteln.

$ kubectl get cronjob

NAME SCHEDULE SUSPEND ACTIVE LAST SCHEDULE AGE

sca-cronjob-cpfiles * * */1 * * False 47 38s 47m

Und dann mit kubectl delete cronjob <name> das Objekt löschen

$ kubectl delete cronjob sca-cronjob-cpfiles

cronjob.batch "sca-cronjob-cpfiles" deleted

**************************************************************

Eduardo Saase

[\\CTS1A519666\public](file://CTS1A519666/public)

start keyloak (roles/group/user

[http://localhost:9090/](http://localhost:9090/)

admin/admin

add client / roles / credentials (set password temp=off)

start wildfly

[http://localhost:9990/console](http://localhost:9990/console)

Iniciar GATO

[https://localhost:8443/](https://localhost:8443/)

anita/anita

edsasse/edsasse/

telnet

open

Iniciar WSPDOKU

- change cacerts

- change context roots to /wspdoku (application.xml inside ear/meta-inf)

- download openjws (java web start deprecated)

- [https://localhost:8443/wspdoku](https://localhost:8443/wspdoku) download / open

comentar/ descomentar

# Daimlers Loging UI

rse4j.CookieStoreProvider=com.tsystems.rse4j.commons.client.security.impl.oidc.OIDCAuthCookieStoreProvider

com.tsystems.rse4j.commons.client.security.impl.oidc.OIDCAuthCookieStoreProvider.loginEndpoint=https://localhost:8443/wspdoku/rse4j/check-login/

jnlp.WSPDOKU_CODEBASE=https://localhost:8443/wspdoku

# JNLP

# rse4j.CookieStoreProvider=com.tsystems.rse4j.commons.client.security.impl.oidc.OIDCWebstartCookieStoreProvider

[https://localhost:8443/](https://localhost:8443/)

Intellij

Port 8787 - localhost:8787

Breakpoint

Run / Debug Wildfly

Run / Debug Configurations

Remote JVM Debug

localhost 8787

-agentlib:jdwp=transport=dt_socket,server=y,suspend=n,address=8787

Wildfly

-------------------------------

pwd - caminho atual

ls - list

java -version

mvm -version

cd c:/work/repos/git/amsys

mvn clean install -DskipTests=true

cd c:/work/repos/git/gato

-- run

./runserver.bat

diff -qr C:/Work/Python27/ C:/Work/Python27-eduardo/

shift+Ins

------------------------------------------------------------------------------------------------

GIT

------------------------------------------------------------------------------------------------

-- sets the author name and email address respectively to be used with your commits.

git config –global user.name “anita ruegsegger” 

-- obtain a repository from an existing URL.

git clone [https://seu16.gdc-leinf01.t-systems.com/bitbucket/scm/ams4truck/gato.git](https://seu16.gdc-leinf01.t-systems.com/bitbucket/scm/ams4truck/gato.git)

git clone --branch maint/TRUCKS-11344_JFOSS [https://seu16.gdc-leinf01.t-systems.com/bitbucket/scm/ams4truck/feed.git](https://seu16.gdc-leinf01.t-systems.com/bitbucket/scm/ams4truck/feed.git)

[https://seu16.gdc-leinf01.t-systems.com/bitbucket/scm/ams4truck/dockerfiles.git](https://seu16.gdc-leinf01.t-systems.com/bitbucket/scm/ams4truck/dockerfiles.git)

-- clone a branch

git clone --branch maint/2.0.0.0 [https://seu16.gdc-leinf01.t-systems.com/bitbucket/scm/ams4truck/wspdoku.git](https://seu16.gdc-leinf01.t-systems.com/bitbucket/scm/ams4truck/wspdoku.git)

-- change to another branch

$ git checkout maint/2.1.0.0

-- lists all the files that have to be committed.

git status

-- list the version history for the current branch.

git log

-- svn update / Fetch and merge changes on the remote server to your working directory:

git pull

-- sends the committed changes of master branch to your remote repository

git push [variable name] master    

------------------------------------------------------------------------------------------------

GIT MERGE

-- merge maint/2.0.0.0 into your active branch:

git merge maint/2.0.0.0

-- abort merge

git merge --abort

-- inside merge (maint/2.1.0.0 | MERGING) favor all to our change. 594. If you're already in conflicted state, and you want to just accept all of ours:

git checkout --ours .

git add .

git checkout --theirs .

git add .

-- opens conflict editor window

git commit

The right way to complete the commit from the screenshot posted above is to type out the commit message (seen in yellow), which does have a character limit.

Then, by pressing 'esc', git opens a command line at the bottom of this screen.

At this time, by typing ':wq', git then writes the commit and quits the screen, returning to the regular command line.

------------------------------------------------------------------------------------------------

git merge -s ours

-- svn simulation/view of update without changing anything

git fetch

git fetch origin

-- svn commitcd

git push origin maint/2.0.0

:q

Reset current HEAD to the specified state / Resets the index and working tree

git reset --hard

git fetch origin

git reset --hard origin/master

-- update feature branch with maint

------------------------------------------------------------------

create new branch

------------------------------------------------------------------

-- PULL (update feature)

f0fp1176@CTS1A955070 MINGW64 /c/work/repos/git/wspdoku/wspdoku-feature (feature/TRUCKS-11698)

$ git pull

-- CHECKOUT

f0fp1176@CTS1A955070 MINGW64 /c/work/repos/git/wspdoku/wspdoku-feature (feature/TRUCKS-11698)

$ git checkout maint/2.0.0.0

error: Your local changes to the following files would be overwritten by checkout:

        WSP-Doku-Client/pom.xml

        WSP-Doku-EAR/pom.xml

        pom.xml

Please commit your changes or stash them before you switch branches.

Aborting

-- STASH (save local changes)

f0fp1176@CTS1A955070 MINGW64 /c/work/repos/git/wspdoku/wspdoku-feature (feature/TRUCKS-11698)

$ git stash save "localchanges"

Saved working directory and index state On TRUCKS-11698: localchanges

-- CHECKOUT (change to maint)

f0fp1176@CTS1A955070 MINGW64 /c/work/repos/git/wspdoku/wspdoku-feature (feature/TRUCKS-11698)

$ git checkout maint/2.0.0.0

Switched to a new branch 'maint/2.0.0.0'

Branch 'maint/2.0.0.0' set up to track remote branch 'maint/2.0.0.0' from 'origin'.

-- PULL (update maint)

f0fp1176@CTS1A955070 MINGW64 /c/work/repos/git/wspdoku/wspdoku-feature (maint/2.0.0.0)

$ git pull

Already up to date.

-- CHECKOUT (change to feature)

f0fp1176@CTS1A955070 MINGW64 /c/work/repos/git/wspdoku/wspdoku-feature (maint/2.0.0.0)

$ git checkout feature/TRUCKS-11698

Switched to branch 'feature/TRUCKS-11698'

Your branch is up to date with 'origin/feature/TRUCKS-11698'.

-- MERGE (maint to feature)

f0fp1176@CTS1A955070 MINGW64 /c/work/repos/git/wspdoku/wspdoku-feature (feature/TRUCKS-11698)

$ git merge maint/2.0.0

-- PUSH

f0fp1176@CTS1A955070 MINGW64 /c/work/repos/git/wspdoku/wspdoku-feature (feature/TRUCKS-11698)

$ git push

-- CREATE NEW BRANCH (from origin feature/TRUCKS-11698)

f0fp1176@CTS1A955070 MINGW64 /c/work/repos/git/wspdoku/wspdoku-feature (feature/TRUCKS-11698)

$ git checkout -b maint/2.1.0.0 feature/TRUCKS-11698

Switched to a new branch 'maint/2.1.0.0'

f0fp1176@CTS1A955070 MINGW64 /c/work/repos/git/wspdoku/wspdoku-feature (maint/2.1.0.0)

$ cat pom.xml

:wq

f0fp1176@CTS1A955070 MINGW64 /c/work/repos/git/wspdoku/wspdoku-feature (maint/2.1.0.0)

$ mvn versions:set -DnewVersion=2.1.0.0-SNAPSHOT

f0fp1176@CTS1A955070 MINGW64 /c/work/repos/git/wspdoku/wspdoku-feature (maint/2.1.0.0)

$ git push

fatal: The current branch maint/2.1.0.0 has no upstream branch.

To push the current branch and set the remote as upstream, use

    git push --set-upstream origin maint/2.1.0.0

$  git push --set-upstream origin maint/2.1.0.0

Total 0 (delta 0), reused 0 (delta 0), pack-reused 0

remote:

remote: Create pull request for maint/2.1.0.0:

remote:   [https://seu16.gdc-leinf01.t-systems.com/bitbucket/projects/AMS4TRUCK/repos/wspdoku/pull-requests?create&sourceBranch=refs/heads/maint/2.1.0.0](https://seu16.gdc-leinf01.t-systems.com/bitbucket/projects/AMS4TRUCK/repos/wspdoku/pull-requests?create&sourceBranch=refs/heads/maint/2.1.0.0)

remote:

To [https://seu16.gdc-leinf01.t-systems.com/bitbucket/scm/ams4truck/wspdoku.git](https://seu16.gdc-leinf01.t-systems.com/bitbucket/scm/ams4truck/wspdoku.git)

* [new branch]      maint/2.1.0.0 -> maint/2.1.0.0

Branch 'maint/2.1.0.0' set up to track remote branch 'maint/2.1.0.0' from 'origin'.

Note that this is configurable. If you do

$git config --add push.default current

then git push will automatically create the branch in the remote repo if necessary

f your push.default is set to simple or upstream, the upstream setting will make git push, used with no additional arguments, just work.

f0fp1176@CTS1A955070 MINGW64 /c/Work/repos/git/k8s-dev (master)

$ git pull

remote: Counting objects: 26, done.

remote: Compressing objects: 100% (26/26), done.

remote: Total 26 (delta 18), reused 0 (delta 0)

Unpacking objects: 100% (26/26), 3.70 KiB | 10.00 KiB/s, done.

From [https://seu16.gdc-leinf01.t-systems.com/bitbucket/scm/ams4truck/k8s-dev](https://seu16.gdc-leinf01.t-systems.com/bitbucket/scm/ams4truck/k8s-dev)

   cf3f2e8..bceeb35  master     -> origin/master

Updating cf3f2e8..bceeb35

Fast-forward

3atool-060/3atool-config-map.yaml | 6 ++++++

3atool-152/3atool-config-map.yaml | 2 ++

ascot/ascot-config-map.yaml       | 6 +++---

sca/sca-config-map.yaml           | 9 ++++++---

4 files changed, 17 insertions(+), 6 deletions(-)

Here we need to see the difference between

Origin: This is the name of a remote. A remote in Git is a common repository that all team members use to exchange their changes. In most cases, this will be an origin.

Master: This is a branch name where we first initiate git and then we use to make commits.And the changes in the master can pull/push into a remote.

origin/master: This is a remote branch, which has a local branch named master on a remote named origin.

f0fp1176@CTS1A955070 MINGW64 /c/work/repos/git/k8s-int (master)

$ kubectl --help

GIT BASH get POD

- download kublctl context from prod [https://swoeacp-api.dewoe.corpintra.net:32001/](https://swoeacp-api.dewoe.corpintra.net:32001/)

- open git bash

- connect to /c/work/repos/git/k8s-prod

- kubectl get pods -n a4t-wspdoku

- save pod wspdoku-deployment-56578dbddc-jxtq

WINDOWS BASH connect to POD

- open windosw bash C:\Program Files\Git\bin

- doppleclick bash.exe

- copy with rechte maustaste

- kubectl exec -n a4t-wspdoku -it wspdoku-deployment-56578dbddc-jxtqr bash

- kubectl exec -n a4t-sca -it sca-deployment-5f945cb46d-fksck  bash