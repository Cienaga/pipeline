pipeline {
    agent 'Principal'
    triggers {
        cron '* * * * *'
    }
    stages{
        stage('Saludo') {
            steps {
                echo 'Hola'
            }
        }
        stage('Versión') {
            steps {
                echo 'Versión de maven'
            }
        }
        stage('Despedida') {
            steps {
                echo 'Adiós'
            }
        }
    }
    post {
        always {
            echo 'PD: Salgo siempre'
        }
        success {
            echo 'Acabó sin problemas'
        }
        failure {
            echo 'Bufff........'
        }
        changed {
            echo 'Esto ha cambiado'
        }
        unstable {
            echo 'Estoy inestable'
        }
        regression {
            echo 'Antes iba y ahora no voy'
        }
    }
}
