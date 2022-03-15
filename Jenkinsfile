pipeline {
         agent any
         stages {
               stage("root"){
                  steps{
                        sh 'echo "amine22102439" | sudo -S sleep 1 && sudo su'
                  }
               }
                 stage('show docker images available') {
                 steps {
                    sh 'sudo docker images'
                 }
                 }
                 stage('show docker running images') {
                 steps {
                    sh 'sudo docker ps'
                 }
                 }
                 stage('down docker compose') {
                 steps {
                       sh 'sudo docker-compose down -v' 
                 }
                 }
                 stage('down docker compose build') {
                 steps {
                       sh 'sudo docker-compose build'
                 }
                 }
              }
}