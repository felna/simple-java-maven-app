pipeline {
    agent {
        docker {
            image 'maven:3.8.6-adoptopenjdk-11' 
            args '-v /Users/nnovkovic/.m2:/root/.m2' 
        }
    }
    stages {
        stage('Build') { 
            steps {
                sh 'mvn -B -DskipTests clean package' 
            }
        }
    }
}
