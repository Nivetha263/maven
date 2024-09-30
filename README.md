pipeline {
    agent any

    stages {
        stage('stage_1') {
            steps {
                echo 'build application 1'
            }
        }
        stage('stage_2') {
            steps {
                echo 'test application'
                echo 'test application 2'
            }
        }
        stage('stage_3') {
            steps {
                echo 'this is first commit'
                echo 'this is second commit'
                echo 'this is third commit'
            }
        }
        stage('stage_4') {
            steps {
                echo 'deploy application 7'
                echo 'deploy application 6'
                echo 'deploy application 5'
                echo 'deploy application 4'
            }
        }
        stage('stage_5') {
            steps {
                echo 'this is my sec project'
                echo 'this is my first project'
                echo 'this is my third project'
                echo 'this is my fourth project'
                echo 'this is my fifth project'
            }
        }
    }
}
