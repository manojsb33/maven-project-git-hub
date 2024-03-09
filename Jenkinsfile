@Library('my-shared-library') _
pipeline{
    agent any
    stages{
        stage('Git Checkout'){
            steps{
                gitCheckout(
                    branch: "master",
                    url: "https://github.com/manojsb33/maven-project-git-hub.git"
                )
            }
        }
        stage('maven unit test'){
            steps{
                script{
                    mveTest()
                }
            }
        }
    }
}
