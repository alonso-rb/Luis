
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

![FRM NEW MENU](https://user-images.githubusercontent.com/62676424/123704144-9548dc80-d822-11eb-84b0-74c1d8db03c6.jpeg)


Una vez se inicia sesión correctamente se dirige hacia el menú principal, el menú principal tiene 4 botones los cuales permiten al usuario dirigirse a CUATRO partes del programa, las cuales son: registro (permite al gestor registrar a un ciudadano), prechequeo (permite al gestor buscar a un ciudadano, modificar sus datos de ser necesario o crearlos y avanzarlo en la cola) Y monitoreo (permite ver si hay alguien en cola, registrar el momento en el que llega al monitoreo, avanzarlo a vacunación y posterior a ello, a observación donde se registra la cita para la segunda dósis).

#### **Formulario: Registro**

![RegistroCiudadanos](https://user-images.githubusercontent.com/62676424/123672393-7fc0bc00-d7fc-11eb-8d60-1049e76b2cc9.jpeg)

Al escoger la opción de registro en el menú, se ingresa hacia el formulario Registro, ahí se deberá completar correctamente los datos que se solicitan; de manera obligatoria se debe completar: número de DUI (sin guion y recordando que los números de DUI y tienen nueve dígitos), nombre de la persona, dirección actual, número de teléfono (sin guion y recordando que los teléfonos tiene ocho dígitos) y la fecha de nacimiento de la persona; de manera opcional se debe completar el correo electrónico, si pertenece a una institución de prioridad deberá completar el número identificador y seleccionar a la institución a la que pertenece con la barra desplegable "Escoja la institución" (de pertencer a una institución, es imperativo que ingrese el número identificador y seleccione la institución, si uno de los dos datos falta, no le permitirá avanzar), y finalmente seleccionar los recuadros correpondientes a las enfermedades crónicas que padece, de no padecer ninguna, simplemente no seleccionar ninguna opción.

Abajo de los datos a solicitar hay dos botones, el primero , de izquierda a derecha, es generar PDF, el segundo es el botón Guardar. 

El botón Guardar permite registrar al ciudadano en el sistema, al igual que registrar su cita, de haber llenado adecuadamente el formulario, aparecerá un cuadro de diálogo, anunciando el éxito de la operación.

![RegCiudaÉxito](https://user-images.githubusercontent.com/62676424/123703512-b4933a00-d821-11eb-998b-f0a892afbe1b.jpeg)

El botón generar PDF permite generar y guardar en la computadora un documento PDF, esto se podrá hacer únicamente si usted ha registrado al usuario con anticipación, de lo contrario, dará error.

![GenerarPDFCiudadano](https://user-images.githubusercontent.com/62676424/123703742-0b007880-d822-11eb-8194-094762ce5900.jpeg)

#### **Formulario: Prechequeo**







