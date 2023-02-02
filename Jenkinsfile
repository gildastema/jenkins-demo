pipeline{
    agent {
        docker{ image 'openjdk:17-alpine'}
    }

    stages {
        stage("Test"){
            steps{
                sh 'chmod +x ./gradlew'
                sh './gradlew check'
            }
            
        }
        stage("Build"){
            steps{
                echo "Building"
            }
        }

    }
}