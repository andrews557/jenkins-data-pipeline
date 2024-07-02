pipeline {
    agent any
    environment {
       PYTHON_HOME = 'C:\Users\andre\AppData\Local\Microsoft\WindowsApps'
        PATH = "${env.PATH};${env.PYTHON_HOME}"
   }
    stages {
        stage('Build') {
            steps {
                script {
                    // Choisissez la commande en fonction de votre script
                   bat "pip install pandas" // Installer les dépendances
                   bat "python data_analysis.py" // Exécuter le script Python
                }
            }
        }
    }
}