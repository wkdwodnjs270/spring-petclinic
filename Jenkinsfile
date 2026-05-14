pipeline {
    agent any

    stages {
        stage('Git Clone') {
            steps {
                echo 'Git Clone'
                git url: 'https://github.com/wkdwodnjs270/spring-petclinic.git',
                branch: 'main'
            }
        }
    }
}
