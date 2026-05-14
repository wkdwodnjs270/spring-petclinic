pipeline {
    agent any

    tools { 
        jdk 'JDK21'
        maven 'M3'
    }   
    
    stages {
        stage('Git Clone') {
            steps {
                echo 'Git Clone'
                git url: 'https://github.com/wkdwodnjs270/spring-petclinic.git',
                branch: 'main'
            }
        }

        //Maven으로 Build
        stage('Maven Build) {
            steps {
                sh 'mvn -Dmaven.test.failure.ignore=true clean package'
            }
        }
    }
}             
