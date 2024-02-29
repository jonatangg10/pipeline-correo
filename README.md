<p align="center">¡ Bienvenido !</p>
<p align="center"><b>Ejemplo practico de Jenkins</b></p>
<p align="center"><a>Dessarrollo un <b>Pipeline</b> para un proceso de notificación a correo electrónico</b></a></p>
<p align="center"><b>Si se puede inmaginar, se puede programar</b></p>

environment {
        LANG = 'es_CO.UTF-8'
        repoLink = 'https://github.com/jonatangg10/pipeline-correo.git'
        destinatario = params.Notificar
    }
    stages {
        stage('Configuración') {
            steps {
                script {
                    echo "Notificar al equipo seleccionado: ${env.destinatario}"
                }
            }
        }
    }
