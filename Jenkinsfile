@Library("belajar-jenkins-shared-library@main") _

import programmerzamannow.jenkins.Output;

pipeline {
  agent any
  stages {
    stage("Library Resource") {
      steps {
        script {
          def config = libraryResource("config/build.json")
          echo(config)
        }
      }
    }
    stage("Hello Person") {
      steps {
        script {
          hello.person([
            firstName: "Eko",
            lastName: "Khannedy"
          ])
        }
      }
    }
    stage("Maven Build") {
      steps {
        script {
          maven(["clean", "compile", "test"])
        }
      }
    }
    stage("Global Variable") {
      steps {
        script {
          echo(author())
          echo(author.name())
          echo(author.channel())
        }
      }
    }
    stage("Hello Groovy") {
      steps {
        script {
          Output.hello(this, "Groovy")
        }
      }
    }
    stage("Hello World") {
      steps {
        script {
          hello.world()
        }
      }
    }
  }
}