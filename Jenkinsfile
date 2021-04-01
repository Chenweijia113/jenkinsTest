pipeline {
    agent { docker 'python:3.8.6-alpine' }
    stages {
        stage('build') {
            steps {
                sh 'echo "hello python!"'
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
