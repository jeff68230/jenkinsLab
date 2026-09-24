pipeline {
    agent any
    stages {
        stage('Compilation & Tests') {
            parallel {
                stage('Build') {
                    steps {
                        echo "Compilation en cours..."
                        sh 'sleep 3' // Simulation du build
                    }
                }
                stage('Tests Unitaires') {
                    steps {
                        echo "Exécution des tests unitaires..."
                        sh 'sleep 2' // Simulation des tests unitaires
                    }
                }
                stage('Analyse Qualité') {
                    steps {
                        echo "Analyse statique du code avec SonarQube..."
                        sh 'sleep 4' // Simulation de l’analyse
                    }
                }
            }
        }
    }
}
