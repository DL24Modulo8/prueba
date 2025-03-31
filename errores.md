Started by user Blanca Pinot

Obtained Jenkinsfile from git https://github.com/DL24Modulo8/prueba.git
[Pipeline] Start of Pipeline
[Pipeline] node
Running on Jenkins
 in /var/jenkins_home/workspace/Prueba8
[Pipeline] {
[Pipeline] stage
[Pipeline] { (Declarative: Checkout SCM)
[Pipeline] checkout
Selected Git installation does not exist. Using Default
The recommended git tool is: NONE
No credentials specified
 > git rev-parse --resolve-git-dir /var/jenkins_home/workspace/Prueba8/.git # timeout=10
Fetching changes from the remote Git repository
 > git config remote.origin.url https://github.com/DL24Modulo8/prueba.git # timeout=10
Fetching upstream changes from https://github.com/DL24Modulo8/prueba.git
 > git --version # timeout=10
 > git --version # 'git version 2.39.5'
 > git fetch --tags --force --progress -- https://github.com/DL24Modulo8/prueba.git +refs/heads/*:refs/remotes/origin/* # timeout=10
 > git rev-parse refs/remotes/origin/dev^{commit} # timeout=10
Checking out Revision 50fb0d061b1bdb68af3b5174e995c75f465626c5 (refs/remotes/origin/dev)
 > git config core.sparsecheckout # timeout=10
 > git checkout -f 50fb0d061b1bdb68af3b5174e995c75f465626c5 # timeout=10
Commit message: "jenkinsfile modifica sh por bat"
 > git rev-list --no-walk 2ce1e6cc3b0d6ff142bc5959aea4741c23c0d84c # timeout=10
[Pipeline] }
[Pipeline] // stage
[Pipeline] withEnv
[Pipeline] {
[Pipeline] withEnv
[Pipeline] {
[Pipeline] stage
[Pipeline] { (Checkout)
[Pipeline] echo
📥 Clonando el repositorio...
[Pipeline] checkout
Selected Git installation does not exist. Using Default
The recommended git tool is: NONE
No credentials specified
 > git rev-parse --resolve-git-dir /var/jenkins_home/workspace/Prueba8/.git # timeout=10
Fetching changes from the remote Git repository
 > git config remote.origin.url https://github.com/DL24Modulo8/prueba.git # timeout=10
Fetching upstream changes from https://github.com/DL24Modulo8/prueba.git
 > git --version # timeout=10
 > git --version # 'git version 2.39.5'
 > git fetch --tags --force --progress -- https://github.com/DL24Modulo8/prueba.git +refs/heads/*:refs/remotes/origin/* # timeout=10
 > git rev-parse refs/remotes/origin/dev^{commit} # timeout=10
Checking out Revision 50fb0d061b1bdb68af3b5174e995c75f465626c5 (refs/remotes/origin/dev)
 > git config core.sparsecheckout # timeout=10
 > git checkout -f 50fb0d061b1bdb68af3b5174e995c75f465626c5 # timeout=10
Commit message: "jenkinsfile modifica sh por bat"
[Pipeline] }
[Pipeline] // stage
[Pipeline] stage
[Pipeline] { (Build)
[Pipeline] script
[Pipeline] {
[Pipeline] echo
⚙️ Instalando dependencias...
[Pipeline] bat
[Pipeline] error
[Pipeline] }
[Pipeline] // script
[Pipeline] }
[Pipeline] // stage
[Pipeline] stage
[Pipeline] { (Test)
Stage "Test" skipped due to earlier failure(s)
[Pipeline] getContext
[Pipeline] }
[Pipeline] // stage
[Pipeline] stage
[Pipeline] { (Deploy)
Stage "Deploy" skipped due to earlier failure(s)
[Pipeline] getContext
[Pipeline] }
[Pipeline] // stage
[Pipeline] stage
[Pipeline] { (Declarative: Post Actions)
[Pipeline] echo
❌ El pipeline ha fallado
[Pipeline] }
[Pipeline] // stage
[Pipeline] }
[Pipeline] // withEnv
[Pipeline] }
[Pipeline] // withEnv
[Pipeline] }
[Pipeline] // node
[Pipeline] End of Pipeline
ERROR: ❌ Error en la etapa de Build
Finished: FAILURE
