pipeline {
    agent any 

    stages {
        stage('Checkout') {
            steps {
                git url: 'https://github.com/MolkaBenJeddou/MolkaBenJeddou.git', branch: 'main' // Assure-toi que la branche est correcte
            }
        }
        stage('Build') {
            steps {
                sh 'mvn clean package' // Assure-toi que Maven est installé sur Jenkins
            }
        }
    }
}
