pipeline {
         agent any
         stages {
                 stage('show docker images available') {
                 steps {
                     sudo docker images
                 }
                 }
                 stage('show docker running images') {
                 steps {
                    sudo docker ps
                 }
                 }
                 stage('down docker compose') {
                 steps {
                       sudo docker-compose down -v 
                 }
                 }
                 stage('down docker compose build') {
                 steps {
                       sudo docker-compose up --build
                 }
                 }
              }
}