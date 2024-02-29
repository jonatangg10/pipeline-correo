<p align="center">¡ Bienvenido !</p>
<p align="center"><b>Ejemplo practico de Jenkins</b></p>
<p align="center"><a>Dessarrollo un <b>Pipeline</b> para un proceso de notificación a correo electrónico</b></a></p>
<p align="center"><b>Si se puede inmaginar, se puede programar</b></p>

def destinatario = params.Notificar == 'Equipo 1' ? 'Hola' : 'adios'
                            echo "Notificar al equipo seleccionado: ${destinatario}"
