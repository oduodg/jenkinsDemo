pipeline {
    agent {
        label "demoAgent"
    }
    tools {
        jdk('JAVA_HOME')
        maven('M2_HOME')
    }
    stages {
        stage('Build') {
            steps {
                echo 'Building..'
            }
        }
        stage('Test') {
            steps {
                build 'SeleniumMaven'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
    post {
        always {
            echo "202206071443"
        }
    }    
}
