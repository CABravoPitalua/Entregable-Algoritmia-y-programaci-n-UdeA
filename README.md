# Entregable Algoritmia y programación UdeA

Actividad evaluativa del currso Algoritmia y programación para ingenieros de la Universidad de Antioquia, cuyo propósito es realizar un software con lenguaje Python para gestionar préstamos de materiales

# 1 y 2.Integrantes - Descripción
**Camila Andrea Bravo Pitalua**

Tras no llegar a un acuerdo de compromisos con los compañeros del grupo de estudio para realizar el trabajo, lo realizaré de manera individual por lo tanto realizaré todas las actividades que determinen el éxito de la actividad.
Soy estudiante de Ingeniería Industrial, considero que mis habilidades y fortalezas son ser una persona responsable, comprometida y proactiva.

# 3. BravoGestor
El nombre que he elegido es el siguiente: 

<img width="300" height="300" alt="image" src="https://github.com/user-attachments/assets/47ad1c27-f548-464c-ad05-c966365a6e84" />

Nota: La illustración es generada con IA

# 4.licencia

# 5. Reporte de visión

Este proyecto se basa en crear una copnsola para la gestion de prestamo de materiales, el cual debe realiazr las siguientes funciones: 

1. Registrar usuarios
2. Registrar materiales
3. Registrar prestamos
4. Registrar devoluciones
5. Generar certificado de devolución
6. Generar notificación de devolución
7. Notificar prestamos con más 20 días
8. Generar factura de venta para prestamos mayores a 30 días
9. Administrador
10. Salir

**Objetivo**

El objetivo del proyecto se basa en desarrollar un sistema de consola que ayude al usuario a gestionar préstamos de materiales, el cual permita registrar usuarios, materiales, gestionar los tiempos de préstamo y devolución.
Realizando este poyecto, el alumno podrá evaluar el aprendizaje del curso y poner en marcha lo aprendido en el trasncurso del semestre, a su vez el profesor determinará si el estudiate cumple con las espectativas para aprobar el curso y realizar el respectivo acompañamiento en la etapa de aprendizaje. 

 **Beneficios**
 
Los beneficios que esperan para el administrador de la consola son los siguientes: 
Mejorar el orden y control de prestamos y devoluciones, reduior errores, facilitar información, hacer seguimiento de usuarios y materiales.

# 6. Especificación de requisitos

**Funcionales**

**1. Regristrar Usuarios**
El usuario debe quedar registrado en el sistema con los siguientes datos básicos:
- Nombre, este debe tener las siguientes validaciones de ingreso de información:
  * Longitud, no menor a tres letras
  * Números, no puede contener números
- Apellido, este debe tener las siguientes validaciones de ingreso de información:
  * Longitud, no menor a tres letras
  * Números, no puede contener números
- Documento, este debe tener las siguientes validaciones de ingreso de información:
  * Longitud, debe contener entre 8 y 10 digitos
  * Numeros, el documento solo debe contener números, no se permite el ingreso de letras u otros caracteres
- Correo electronico, este debe tener la validación de correo electronico, contener un "@" y debe terminar con "." y "com".
- Tiempo de préstamo definido a la hora de crear el usuario, se deben ingresar valores entre 1 a 30 días, otros valores no está permitido.
  
**2. Regristrar Materiales (objetos a prestar)**
BravoGestor deberá registrar cada material a prestar, este debe estar categorizado correctamente:
- Nombre, este debe tener las siguientes validaciones de ingreso de información:
  * Longitud, no menor a tres letras
  * Números, no puede contener números
- Categoría, el material debe estar categorizado entre los siguientes tipos de objetos: 
Juegos o Herramietas o Electrodomesticos o varios 
- Precio de compra, se debe registrar el precio de compra del material. 
-	ID del material, se debe crear un identificador único para cada material con combinaciones entre letras y números, se debe usar la categoría para asociar el ID con el material. 
-	Estado del material, se debe dar una valoración del estado del material a prestar, se debe utilizar lógica difusa para registrar la calidad o estado del material. 

**3. Registrar Prestamos**
- El programa deberá verificar que el ususario este registrado antes de registrar el prestamo, en caso que el usuario no esté registrado debe emitir un mensaje de error.
- El programa deberá permitir seleccionar el material a prestar mediante su ID o código identificador.
- El programa deberá registrar la fecha del prestamo
- El programa deberá relacionar el préstamo con el usuario y el material correspondiente.

**4. Registrar Devoluciones**
- El programa deberá validar que el usuario tenga prestamos activos.
- El programa deberá registrar la fecha de la devolución
- El programa deberá actualizar el estado del material a disponible una vez sea devuelto.
- El programa deberá impedir registrar devoluciones de préstamos inexistentes.
- El programa deberá mostrar un mensaje de validación cuando no existan préstamos activos para ese usuario.

**5. Generar certificado de devolución**
- El programa debera generar un certificado cuando se registre la devolución del material.
- El programa debera incluir los datos del usuario, datos del material y la fecha de la devolución

**6. Generar notificación de devolución.**

**7. Notificar prestamos con más 20 días.**
- El programa dederácalcular cuantos días han transcurrido desde la fecha inicial del prestamo.
- El programa deberá filtrar los prestamos que superen los 20 días de duración
- El programa debera general una notoficación de un aviso de solicitud de devolución
- El programa deberá mostrar en la notificación la información del usuario y del material que se solicita devolver



5. Registrar devoluciones
6. Acceso administrador

**No funcionales**
1. Rendimiento
2. Compatibilidad
3. Legibilidad
4. Seguridad

# 7. Plan del proyecto
1. Definir el problema, sus variables, parametros (Hacer una notación de ser posible)
2. Estimar un cronograma
3. Presupuesto




