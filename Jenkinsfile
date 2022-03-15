pipeline {
         agent any
         stages {
                 stage('show docker images available') {
                 steps {
                    sh 'docker images'
                 }
                 }
                 stage('show docker running images') {
                 steps {
                    sh 'docker ps'
                 }
                 }
                 stage('down docker compose') {
                 steps {
                       sh 'docker-compose down -v' 
                 }
                 }
                 stage('down docker compose build') {
                 steps {
                       sh 'docker-compose build'
                 }
                 }
              }
}