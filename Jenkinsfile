pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git url: 'https://github.com/MolkaBenJeddou/MolkaBenJeddou.git', credentialsId: 'github'
            }
        }
        stage('Build') {
            steps {
                // Ici, tu peux ajouter des étapes pour compiler ton projet
                sh 'mvn clean package' // Assure-toi que Maven est installé sur Jenkins
            }
        }
    }
}
