#!groovy

// https://github.com/feedhenry/fh-pipeline-library
@Library('fh-pipeline-library') _

stage('Enforce trusted approval') {
    enforceTrustedApproval('grdryn-test-org', 'github-grdryn')
}

stage('Build') {
    node {
        println "it's alive!"
        sh "env"
        println "===="
        println params
    }
}
