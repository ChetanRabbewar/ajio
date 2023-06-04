pipeline {
agent any 
stages{
stage('Checkout'){
steps{
checkout scm
}}
stage('Build'){
steps{
sh '/home/chetan/Documents/softdev/apache-maven-3.9.1/bin/mvn install'
}}
stage('Deployment'){
steps{
sh 'cp target/ajio.war /home/chetan/Documents/softdev/apache-tomcat-9.0.73/webapps'
}}
}} 
