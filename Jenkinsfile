pipeline {
    agent any
    environment {
       "PYTHON_HOME = /usr/bin"
       "PATH = ${env.PATH};${env.PYTHON_HOME}"
   }
    stages {
        stage('Build') {
            steps {
                script {
                    // Choisissez la commande en fonction de votre script
                   sh "pip install pandas" // Installer les dépendances
                   sh "python data_analysis.py" // Exécuter le script Python
                }
            }
        }
    }
}
