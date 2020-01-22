pipeline {
 agent any
 tools {
 maven 'maven'
 jdk 'jdk'
 }
 stages{
 stage ('build') {
 steps {
 echo "code is building"
 sh 'mvn clean'
 sh 'mvn install'
 }
 }
 stage ('running playbook') {
 steps {
 sh 'ansible-playbook tomcat.yml'
 }
 }
 }
 }
