pipeline{
    agent {
        docker{
            image 'openjdk:17-alpine'
        }
    }

    stages {
        stage("Test"){
            steps{
                chmod +x ./gradlew
                ./gradlew check
            }
            
        }
        stage("Build"){
            steps{
                echo "Building"
            }
        }

    }
}