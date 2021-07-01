
# **DOCUMENTACIÓN** **OFICIAL**
***
##  Aspectos técnicos del programa

> ###  **Softwares instalados**

**Visual Studio Community 2019.** Versión del software: 16.10.2.

**MySQL Server.** Versión del software: 8.0.19.

**MySQL Workbench.** Versión del software: 8.0.19.

> ### **Patrones de diseño**

**View Model**: El patrón de diseño view model fue utilizado en nuestro proyecto, esto debido a la organización y facilidad que otorga al trabajar, con todos los forms que se generaron en una sola carpeta (View), permite que todas las interfaces gráficas estén agrupadas y sea más fácil de trabajar con ellas.

> ### **Paquetes externos**

**Itext7.** Versión del paquete: 7.1.15.

**ItextSharp.** Versión del paquete: 5.5.13.2.

**MySql.EntityFrameworkCore.** Versión del paquete: 5.0.3.1.

**Microsoft.EntityFrameworkCore.** Versión del paquete: 5.0.7.

**Microsoft.EntityFrameworkCore.Design.** Versión del paquete: 5.0.7.

## **Manual de Usuario**

> ### **Descripción general del software**

A raíz de la pandemia del Covid 19, el Gobierno de El Salvador con el fin de proteger la salud de la población ha comenzado la gestión del proceso de vacunación en todo el país, para ellos, se necesita un software que sea permita facilitar ese proceso. Para solventar esa necesidad se ha creado el software "Cabina de vacunación", el cual gestiona el proceso de vacunación de una persona a través de un usuario que administra el programa (conocido como gestor), para ingresar al sistema, el gestor debe iniciar sesión colocando correctamente el nombre de usuario y contraseña que se han establecido para él Una vez ingresado al sistema, se le presenta al gestor, un menú con tres opciones disponibles, la primera registrar al usuario, la segunda prechequeo, la tercera monitoreo de citas. Si el usuario escoge registro, una vez complete los campos necesarios, podrá registrar al usuario, registrar la cita, y obtener los datos de la misma. Si el usuario escoge prechequeo tendrá la opción de buscar un usuario, completar o modificar sus datos de ser necesario, avanzarlo en la fila, registrar su proceso de vacunación y finalmente asignarle una segunda cita. Al finalizar cualquiera de los dos procesos, el gestor puede regresar al menú principal, en la que, podrá presionar el botón de cerrar sesión para salir de su sesión y finalizar el programa.

>### **Formularios**

A continuación se presentarán los 7 formularios junto con su descripción, funcionalidad e instrucciones de uso.

#### **Formulario: Inicio de Sesión**

![InicioSesion](https://user-images.githubusercontent.com/62676424/123669058-f1970680-d7f8-11eb-834e-bea6df45e98a.jpeg)

El programa comienza con "Inicio de Sesión", el cual, le permite al gestor colocar su nombre de usuario y contraseña para iniciar sesión en la plataforma y utilizarla. Es imperativo que el usuario coloque correctamente sus datos, caso contrario, no podrá ingresar a la plataforma.

#### **Formulario: Menú**

![menu](https://user-images.githubusercontent.com/62676424/124159469-6fa51880-da58-11eb-82ed-84eeda460311.png)

Una vez se inicia sesión correctamente se dirige hacia el menú principal, el menú principal tiene 4 botones los cuales permiten al usuario dirigirse a cuatro partes del programa, las cuales son: empleados (permite al gestor visualizar la lista de empleados y buscar los datos de uno), registro (permite al gestor registrar a un ciudadano), prechequeo (permite al gestor buscar a un ciudadano, modificar sus datos de ser necesario o crearlos y avanzarlo en la cola) Y monitoreo (permite ver si hay alguien en cola, registrar el momento en el que llega al monitoreo, avanzarlo a vacunación y posterior a ello, a observación donde se registra la cita para la segunda dosis).

#### **Formulario: Empleados**

![empl](https://user-images.githubusercontent.com/62676424/124160621-ad567100-da59-11eb-97ae-59eb1e57dd5c.png)

Al escoger la opción empleados en el menú, el gestor podrá visualizar un listado con todos los empleados. El gestor, podrá buscar un empleado en particular, ingresando su ID en el cuadro de texto y presionando el botón de buscar, una vez encontrado, se visualizarán únicamente los datos de dicho empleado.

#### **Formulario: Registro**

![RegistroCiudadanos](https://user-images.githubusercontent.com/62676424/123672393-7fc0bc00-d7fc-11eb-8d60-1049e76b2cc9.jpeg)

Al escoger la opción de registro en el menú, se ingresa hacia el formulario Registro, ahí se deberá completar correctamente los datos que se solicitan; de manera obligatoria se debe completar: número de DUI (sin guion y recordando que los números de DUI tienen nueve dígitos), nombre de la persona, dirección actual, número de teléfono (sin guion y recordando que los teléfonos tiene ocho dígitos) y la fecha de nacimiento de la persona; de manera opcional se debe completar el correo electrónico, si pertenece a una institución de prioridad deberá completar el número identificador y seleccionar a la institución a la que pertenece con la barra desplegable "Escoja la institución" (de pertenecer a una institución, es imperativo que ingrese el número identificador y seleccione la institución, si uno de los dos datos falta, no le permitirá avanzar), y finalmente seleccionar los recuadros correspondientes a las enfermedades crónicas que padece, de no padecer ninguna, simplemente no seleccionar ninguna opción

Abajo de los datos a solicitar hay dos botones, el primero , de izquierda a derecha, es generar PDF, el segundo es el botón Guardar. 

![boton pdf y guardar](https://user-images.githubusercontent.com/62676424/124163580-ecd28c80-da5c-11eb-8efc-b2b4e95da4ab.png)

El botón Guardar permite registrar al ciudadano en el sistema, al igual que registrar su cita, de haber llenado adecuadamente el formulario, aparecerá un cuadro de diálogo, anunciando el éxito de la operación. El botón generar PDF permite generar y guardar en la computadora un documento PDF, esto se podrá hacer únicamente si usted ha registrado al usuario con anticipación, de lo contrario, dará error.

#### **Formulario: Prechequeo**

![pRECHEQUEO](https://user-images.githubusercontent.com/62676424/124164192-b0536080-da5d-11eb-88a7-a705047a653b.jpg)

El formulario contiene en la parte superior en la que debe ingresar el ID del ciudadano a buscar (este ID debe estar registrado y no es válido colocar caracteres que no le corresponden al ID), una vez se coloque el ID que corresponde al ciudadano y se presione buscar, aparecerán los datos del ciudadano.
Si el usuario colocó un dato equivocado en su registro, el gestor podrá corregírselo. Una vez, se verifiquen los datos, debe asegurarse que la persona de su consentimiento para recibir la dosis, caso contrario, no lo dejará avanzar.

![PRECHEQUEO EXITO](https://user-images.githubusercontent.com/62676424/124164577-0d4f1680-da5e-11eb-8dac-c192189e20c2.png)

Una vez el ciudadano ha dado su consentimiento y se selecciona dicha casilla, aparecerá un cuadro de diálogo cuyo título será "operación exitosa", que indicara que el ciudadano ha sido ingresado a la cola. Para continuar con monitoreo de citas, deberá dar clic en volver, el cual le redirigirá al menú principal.

#### **Formulario: Monitoreo de citas**

![citasss](https://user-images.githubusercontent.com/62676424/124166581-438d9580-da60-11eb-9860-a7f610dd6819.png)

Al escoger la opción monitoreo en el menú principal, se encontrará con la ventana, monitoreo de citas, ahí, se tendrá acceso a la cola de pacientes esperando por avanzar en su proceso, para avanzar al ciudadano en la cola, el gestor podrá seleccionar el botón con la flecha que se encuentra a la izquierda del DUI del ciudadano que desea avanzar y podrá agregarlo a la lista.

#### **Formulario: Registro de vacunación**

![RegistroVacunacion](https://user-images.githubusercontent.com/62676424/124166726-733c9d80-da60-11eb-9c1b-08cd0391360a.jpg)

Una vez se avance al ciudadano en la cola, se dirigirá al registro de vacunación, al ser vacunado el ciudadano, se deberá presionar el botón "vacunado". Al presionar el botón, habrá un tiempo de espera, cuando este termine, la barra indicará al completarse de color verde y aparecerá un cuadro de diálogo mencionando que el tiempo de observación ha terminado.

#### **Formulario: Observación**

![Observation](https://user-images.githubusercontent.com/62676424/124181471-c28bc980-da72-11eb-8b78-3ea5d70800b1.png)


Como último paso, se avanzará al ciudadano a observación, donde tendrá que seleccionar al ciudadano y seleccionar cuál o cuáles son los efectos secundarios que presenta después que se le haya aplicado la vacuna.  En caso de no haber ninguno, no se seleccionará nada. Independientemente el ciudadano presente o no efectos secundarios, se deberá presionar el botón agregar efectos. El botón agrega los efectos secundarios y también permite agendar la segunda cita del ciudadano. 

Del gestor y el usuario necesitarlo, se podrá generar un PDF que indique los datos del ciudadano, los efectos secundarios que presentó y el detalle de su segunda cita.



| Error      |                                                       Descripción                                                       | Imagen |
|------------|:--------------------------------------------------------------------------------------------------------------------:|:-----------:|
| Inicio de Sesión | Como se había mencionado al explicar cada formulario, es imperativo que el gestor coloque bien sus datos, caso contrario, aparecerá un cuadro de diálogo que indicará "Error" y no lo dejará avanzar hasta ingresar el nombre de usuario y contraseña correctos. | ![loginerror](https://user-images.githubusercontent.com/62676424/124168142-f90d1880-da61-11eb-8455-49fa3f403187.png)|
| Registro ciudadano |Registro de ciudadanos requiere mucho cuidado al momento de llenar información. Al aparecer el cuadro de diálogo "Asegúrese de llenar la información correctamente", le indica al usuario que un campo está vacío o, en su defecto, que la persona ha agregado un número de identificador pero no ha seleccionado una institución o viceversa. Para solucionarlo, asegúrese de haber llenado los campos obligatorios, que el número de teléfono y número de DUI tengan 8 y 9 dígitos respectivamente y no tener discrepancias en los datos opcionales. También, este error se extiende a no ingresar un ID válido, datos alfabéticos o alfanuméricos como "hola" u "Hola123" no se pueden ingresar, tampoco se puede repetir el registro de un ciudadano previamente registrado, ya que el sistema detectará dos DUIs repetidos, por lo tanto, no dejará registrar por segunda vez al usuario.|![regerror](https://user-images.githubusercontent.com/62676424/124171000-3921ca80-da65-11eb-8e95-f105692dfc25.png)|
| Prechequeo: error 1 |Registro de ciudadanos requiere mucho cuidado al momento de llenar información. Al aparecer el cuadro de diálogo "Asegúrese de llenar la información correctamente", le indica al usuario que un campo está vacío o, en su defecto, que la persona ha agregado un número de identificador pero no ha seleccionado una institución o viceversa. Para solucionarlo, asegúrese de haber llenado los campos obligatorios, que el número de teléfono y número de DUI tengan 8 y 9 dígitos respectivamente y no tener discrepancias en los datos opcionales. También, este error se extiende a no ingresar un ID válido, datos alfabéticos o alfanuméricos como "hola" u "Hola123" no se pueden ingresar, tampoco se puede repetir el registro de un ciudadano previamente registrado, ya que el sistema detectará dos DUIs repetidos, por lo tanto, no dejará registrar por segunda vez al usuario.|![preerror2](https://user-images.githubusercontent.com/62676424/124171395-bf3e1100-da65-11eb-8b50-9c085271b0df.png)|
| Prechequeo: error 2 |Otro error que puede ocurrir se indicará aparecer el cuadro de diálogo con "Algo salió mal con la búsqueda", indica que no ha ingresado ningún DUI para buscar o ha ingresado datos inválidos (caracteres alfabéticos o alfanuméricos).|![preerror1](https://user-images.githubusercontent.com/62676424/124172041-936f5b00-da66-11eb-881c-1cb36b030237.png)|
| Prechequeo: error 3 |Otro error que puede ocurrir se indicará aparecer el cuadro de diálogo con "Algo salió mal con la búsqueda", indica que no ha ingresado ningún DUI para buscar o ha ingresado datos inválidos (caracteres alfabéticos o alfanuméricos).|![preerror1](https://user-images.githubusercontent.com/62676424/124172041-936f5b00-da66-11eb-881c-1cb36b030237.png)|











