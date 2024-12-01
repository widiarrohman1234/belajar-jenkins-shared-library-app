@Library("belajar-jenkins-shared-library@main") _

import widiarrohman.jenkins.Output;

pipeline {
    agent any
    stages{
        stage("Maven Build"){
            steps{
                script{
                    echo 'Stage Maven Build'
                    echo(maven("clean compile"))
                }
            }
        }
        stage("Global Variable"){
            steps{
                script{
                    echo 'Stage Global Variable'
                    echo(author())
                    echo(author.name())
                    echo(author.channel())
                }
            }
        }
        stage("Hello Groovy"){
            steps{
                script{
                    echo 'Stage Hello Groovy'
                    Output.hello(this, 'Groovy :)')
                }
            }
        }
        stage("Hello World"){
            steps{
                script{
                    echo 'Stage Hello World'
                    hello.world()
                }
            }
        }
    }
}