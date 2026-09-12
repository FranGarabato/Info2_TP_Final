# Info 2 - Trabajo Práctico Final
# Caja Fuerte Digital
### Descripción
El objetivo del presente proyecto es la realización de una caja fuerte digital, por medio del desarrollo de una máquina de estados. La caja fuerte tendrá el siguiente funcionamiento: Al presionar el botón de confirmación, se pedirá al usuario el ingreso de cuatro dígitos, correspondientes a la combinación que acciona el mecanismo de apertura de la caja fuerte. Una vez ingresado el código, el usuario volverá a presionar el botón de confirmación. En caso de ser correcto el código ingresado, el cual será de 4 dígitos, la caja fuerte se abrirá, y permanecerá en ese estado hasta que el usuario nuevamente presione el botón de confirmación.
En caso de ingresar una clave incorrecta, el sistema permitirá dos intentos más. Si al tercer intento el usuario no lograse introducir correctamente la clave, ese emitirá una alarma, la cual permanecerá encendida y no permitirá interacción alguna con el sistema durante un periodo determinado de tiempo. Transcurrido dicho periodo volverá al estado de espera.
En la siguiente imagen se puede visualizar el diagrama de estados y transiciones de la máquina de estados:

<div align="center">
  <img src="Diagrama_de_Estados.png" alt="Diagrama de Estados y Transisiones" width="300">
</div>

### Implementación
Se buscará implementar esta máquina por medio de un microcontrolador ESP 32 programado en lenguaje C. Simultáneamente se simulará la apertura de la caja fuerte con una contactora, la cual se activa con la circulación de corriente continua. Si fuese necesario, se agregara una etapa conmutadora con BJT.
El sistema también contará con un display LCD que mostrará los datos ingresados, y un teclado rudimentario con pulsadores.
