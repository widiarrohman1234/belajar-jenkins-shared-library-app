@Library("belajar-jenkins-shared-library@main") _

import widiarrohman.jenkins.Output;

pipeline {
    agent any
    stages{
        stage("Global Variable"){
            steps{
                script{
                    echo(author.name())
                    echo(author.channel())
                }
            }
        }
        stage("Hello Groovy"){
            steps{
                script{
                    Output.hello(this, 'Groovy :)')
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