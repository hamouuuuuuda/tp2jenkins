pipleline {
  agent any
  tools {
    maven 'maven'
  }
  stages {
    stage ("clean up"){
      setps{
        deleteDir()
      }
    }
    stage ("clone repo"){
      setps{
        sh "https://github.com/hamouuuuuuda/tp2jenkins.git"
      }
    }
    stage ("Generate backend image"){
      setps{
        dir ("exp1-spring"){
          sh "mvn clean install"
          sh "docker build -t docexp1-spring"
        }
      }
    }
    stage ("Run docker compose"){
      setps{
       dir ("exp1-spring"){
          sh " docker compose up -d"
        }
    }
