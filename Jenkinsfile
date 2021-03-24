pipeline {
    agent { docker 'python:3.5.1' }
    stages {
        stage('build') {
            steps {
                sh 'python --version'
            }
        }
    }
    post {
        success {
            mail to: '654891551@qq.com',
                 subject: "项目构建成功",
                 body: "项目构建成功了!"
        }
    }
}
