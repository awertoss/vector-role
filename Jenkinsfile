pipeline {
   agent {
       label 'linux'
   }
   stages {
       stage('Git') {
           steps{
               git branch: 'main', credentialsId: '7b188317-b12a-4e64-9c1f-933df2cedf29', url: 'git@github.com:awertoss/vector-role.git'
           }
       }
       stage('Molecule install') {
           steps{
               sh 'pip3 install molecule==3.5.2'
               sh 'pip3 install "ansible-lint<6.0.0"'
               sh 'pip3 install molecule_docker'
           }
       }
       stage('Molecule test'){
           steps{
               sh 'molecule test -s centos'
               cleanWs()
           }
       }
   }
}
