# Entregable Algoritmia y programación UdeA

Actividad evaluativa del currso Algoritmia y programación para ingenieros de la Universidad de Antioquia, cuyo propósito es realizar un software con lenguaje Python para gestionar préstamos de materiales

# 1 y 2. Integrantes - Descripción
**Camila Andrea Bravo Pitalua**

Soy estudiante de Ingeniería Industrial, considero que mis habilidades y fortalezas son ser una persona responsable, comprometida y proactiva.
Tras no llegar a un acuerdo de compromisos con los compañeros del grupo de estudio para realizar el trabajo, lo realizaré de manera individual, por lo tanto realizaré todas las actividades que determinen el éxito de la actividad, las que incluyen el análisis, trabajo de redacción, organización y creación del código.


# 3. BravoGestor
El nombre que he elegido es el siguiente: 

<img width="300" height="300" alt="image" src="https://github.com/user-attachments/assets/47ad1c27-f548-464c-ad05-c966365a6e84" />

Nota: La illustración es generada con IA

# 4.Licencia
Se utilizará la licencia Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International (CC BY-NC-ND 4.0)
Elegí esta licencia para proteger el contenido del proyecto y permitir la autoría a mi persona, que no se use para fines comerciales, ni se puedan realizar modificaciones sin mi consentimiento.

# 5. Reporte de visión

Este proyecto se basa en crear una consola para la gestión de préstamo de materiales, el cual debe realizar las siguientes funciones: 

1. Registrar usuarios
2. Registrar materiales
3. Registrar préstamos
4. Registrar devoluciones
5. Generar certificado de devolución
6. Generar notificación de devolución
7. Notificar préstamos con más de 20 días
8. Generar factura de venta para préstamos mayores a 30 días
9. Administrador
10. Salir

**Objetivo**

El objetivo del proyecto se basa en desarrollar un sistema de consola que ayude al usuario a gestionar préstamos de materiales, el cual permita registrar usuarios, materiales, gestionar los tiempos de préstamo y devolución.
Realizando este proyecto, el alumno podrá evaluar el aprendizaje del curso y poner en marcha lo aprendido en el transcurso del semestre, a su vez el profesor determinará si el estudiante cumple con las expectativas para aprobar el curso y realizar el respectivo acompañamiento en la etapa de aprendizaje. 

 **Beneficios**
 
Los beneficios que se esperan para el administrador de la consola son los siguientes: 
Mejorar el orden y control de préstamos y devoluciones, reducir errores, facilitar información, hacer seguimiento de usuarios y materiales.

# 6. Especificación de requisitos

**Requisitos Funcionales**

**1. Registrar Usuarios**
El usuario debe quedar registrado en el sistema con los siguientes datos básicos:
- Nombre, este debe tener las siguientes validaciones de ingreso de información:
  * Longitud, no menor a tres letras
  * Números, no puede contener números
- Apellido, este debe tener las siguientes validaciones de ingreso de información:
  * Longitud, no menor a tres letras
  * Números, no puede contener números
- Documento, este debe tener las siguientes validaciones de ingreso de información:
  * Longitud, debe contener entre 8 y 10 dígitos
  * Números, el documento solo debe contener números, no se permite el ingreso de letras u otros caracteres
- Correo electrónico, este debe tener la validación de correo electrnico, contener un "@" y debe terminar con "." y "com".
- Tiempo de préstamo definido a la hora de crear el usuario, se deben ingresar valores entre 1 a 30 días, otros valores no está permitido.
  
**2. Registrar Materiales (objetos a prestar)**
BravoGestor deberá registrar cada material a prestar, este debe estar categorizado correctamente:
- Nombre, este debe tener las siguientes validaciones de ingreso de información:
  * Longitud, no menor a tres letras
  * Números, no puede contener números
- Categoría, el material debe estar categorizado entre los siguientes tipos de objetos: 
Juegos o Herramientas o Electrodomésticos o varios 
- Precio de compra, se debe registrar el precio de compra del material. 
-	ID del material, se debe crear un identificador único para cada material con combinaciones entre letras y números, se debe usar la categoría para asociar el ID con el material. 
-	Estado del material, se debe dar una valoración del estado del material a prestar, se debe utilizar lógica difusa para registrar la calidad o estado del material. 

**3. Registrar Préstamos**
El programa deberá:
- Verificar que el usuario esté registrado antes de registrar el prestamo, en caso que el usuario no esté registrado debe emitir un mensaje de error.
- Permitir seleccionar el material a prestar mediante su ID o código identificador.
- Registrar la fecha del prestamo
- Relacionar el préstamo con el usuario y el material correspondiente.

**4. Registrar Devoluciones**
El programa deberá:
- Validar que el usuario tenga prestamos activos.
- Registrar la fecha de la devolución
- Actualizar el estado del material a disponible una vez sea devuelto.
- Impedir registrar devoluciones de préstamos inexistentes.
- Mostrar un mensaje de validación cuando no existan préstamos activos para ese usuario.

**5. Generar certificado de devolución**
El programa deberá:
- Generar un certificado cuando se registre la devolución del material.
- Incluir los datos del usuario, datos del material y la fecha de la devolución en el certificado.

**6. Generar notificación de devolución.**
El programa deberá:
- Emitir un mensaje de aviso cuando el material deba ser devuelto
- Relacionar el mensaje con el usuario y el material correspondiente

**7. Notificar prestamos con más de 20 días.**
El programa deberá:
- Calcular cuántos días han transcurrido desde la fecha inicial del prestamo.
- Filtrar los prestamos que superen los 20 días de duración
- Generar una notificación de un aviso de solicitud de devolución
- Mostrar en la notificación la información del usuario y del material que se solicita devolver

**8. Generar factura de venta para prestamos mayores a 30 días**
El programa deberá:
- Calcular cuántos días han transcurrido desde la fecha inicial del prestamo.
- Filtrar los prestamos que superen los 30 días de duración
- Identificar el precio de compra del material
- Generar una factura con los datos del usuario y del material

**9. Administrador**
El programa debe contar con un módulo de administrador protegido por usuario y contraseña, para acceder al sistema el programa debe validar estos datos y restringir el acceso si los datos son erróneos.
El administrador debe tener acceso a los prestamos, las devoluciones, ventas, lista de usuarios y el inventario de los materiales


**Requisitos No funcionales**

**1. Rendimiento**
El programa debe responder de manera rápida al registrar, consultar y actualizar información sobre los parámetros y variables

**2. Compatibilidad**
El programa será desarrollado con lenguaje Python y se ejecutará en Visual Studio Code (VSC).

**3. Legibilidad**
Este proyecto se está redactando en Markdown en forma estructurada y secciones definidas para facilitar su revisión.

**4. Seguridad**
El acceso de administrador se protegerá con usuario y contraseña.

**5. Usabilidad**
El menú de la consola debe tener un menu claro, ordenado y de fácil acceso a la información para el usuario.

**6. Mantenibilidad**
El proyecto debe desarrollarse de manera organizada para facilitar en un futuro correcciones o mejoras, para permitir incorporar ajustes sin alterar el funcionamiento del programa

# 7. Plan del proyecto
Describe las actividades, el cronograma (Diagrama de Gantt) y el presupuesto del proyecto. 

**Actividades y cronograma**
Para esta primera entrega del proyecto se realizaron las siguientes actividades y el cronograma respecto a las semanas del semestre: 
- Tarea 1: Elegir y descargar la versión de Python y el entorno de desarrollo VSC
- Tarea 2: Definir el problema, sus objetivos y beneficios 
- Tarea 3: Elegir el nombre del proyecto y con ayuda de IA crear una imagen representativa 
- Tarea 4: Redactar los requisitos funcionales y no funcionales 
- Tarea 5: Definir la licencia que se usará en el software 
- Tarea 6: Organizar el repositorio en GitHub 
- Tarea 7: Realizar la primera entrega del trabajo
- Tarea 8: Realizar plan de versionado 
- Tarea 9: Redactar algoritmo 
- Tarea 10: Redactar manual del usuario 
- Tarea 11: Crear un repositorio en GitHub con credenciales UdeA 
- Tarea 12: Presentar la sustentación del proyecto

**Diagrama de Gantt**
<img width="1024" height="768" alt="Gráfico Diagrama de Gantt Profesional Multicolor" src="https://github.com/user-attachments/assets/0ff61546-ddd4-4b9c-8a71-56db0762f8d1" />

**Presupuesto del proyecto**
El presupuesto del trabajo lo voy a medir en tiempo de práctica ya que es académico y no tiene fines de lucro.
Para este proyecto se estima una dedicación total de 50 horas de trabajo.

La distribución estimada del tiempo es la siguiente:

- Tarea 1: Elegir y descargar la versión de Python y el entorno de desarrollo VSC: 0,5 horas
- Tarea 2: Definir el problema, sus objetivos y beneficios: 2 horas 
- Tarea 3: Elegir el nombre del proyecto y con ayuda de IA crear una imagen representativa: 0,5 horas 
- Tarea 4: Redactar los requisitos funcionales y no funcionales : 4 horas
- Tarea 5: Definir la licencia que se usará en el software: 0,3 horas
- Tarea 6: Organizar el repositorio en GitHub: 2 horas
- Tarea 7: Realizar la primera entrega del trabajo (subirlo a la plataforma): 0,2 horas
- Tarea 8: Realizar plan de versionado: 10 horas
- Tarea 9: Redactar algoritmo: 25,5
- Tarea 10: Redactar manual del usuario: 4 horas
- Tarea 11: Crear un repositorio en GitHub con credenciales UdeA: 0,5 horas
- Tarea 12: Presentar la sustentación del proyecto: 1 hora
Total estimado: 50 horas

