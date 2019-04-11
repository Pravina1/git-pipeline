<<<<<<< Updated upstream
    pipeline {
        agent any
        stages {
            stage('Checkout from git ') {
                steps {
                    echo "checking out from git"    
                    checkout([$class: 'GitSCM', branches: [[name: '*/feature2']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: '927d86e3-03fd-468c-a3e6-063f6771cea4', url: 'https://github.com/Pravina1/git-pipeline.git']]])
=======
pipeline {
    agent any
    stages {
        stage('Checkout from git ') {
            steps {
                echo " hi ..checking out from git"    
                checkout([$class: 'GitSCM', branches: [[name: '*/feature3']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: '927d86e3-03fd-468c-a3e6-063f6771cea4', url: 'https://github.com/Pravina1/git-pipeline.git']]])
            }
            }
        stage('clean') {
            steps {
                sh "mvn clean"
>>>>>>> Stashed changes
                }
                }
            stage('clean') {
                steps {
                    sh "mvn clean"
                    }
                }
            stage('compile') {
                steps {
                    echo 'compiling src....'
                    sh "mvn compile"
                    }
                }
            stage('package') {
                steps {
                    sh "mvn package"
                      }
                }
            stage('deploy') {
                steps {
                    sh "mvn deploy"
                    }
                }
            }
        }

