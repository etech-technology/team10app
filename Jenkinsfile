pipeline{
    agent any
    stages{
        stage('1-clone-codes'){
            steps{
                checkout scmGit(branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[credentialsId: 'job_id', url: 'https://github.com/etech-technology/team10app']])
            }
        }
        stage('3-disk-usage'){
            steps{
                sh 'du -h'
            }
        }
    }
}