pipeline{
    agent any
    stages{
        stage('1-clone-codes'){
            steps{
                checkout scmGit(branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[credentialsId: 'new_id', url: 'https://github.com/etech-technology/team10app']])
            }
        }
        stage('2-system-check'){
            steps{
                sh 'cat /etc/passwd'
            }
        }
        stage('3-disk-usage'){
            steps{
                sh 'du -h'
            }
        }
    }
}