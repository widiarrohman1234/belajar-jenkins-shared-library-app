@Library("belajar-jenkins-shared-library@main") _

import widiarrohman.jenkins.Ouput;

pipeline {
    agent any
    stages{
        stage("Hello Groovy"){
            steps{
                script{
                    Ouput.hello('Groovy :)')
                }
            }
        }
        stage("Hello World"){
            steps{
                script{
                    hello.world()
                }
            }
        }
    }
}