# HolaMundoFinal - Especificaciones de Requerimientos de Software
Preparado por: Andrea Bellesia, Sara Visoso, Israel Cabrera, Victor Manual Jiménez 

Link Proyecto: https://asesorias-online-holamundo.herokuapp.com/login

# Tabla de contenido 
1. [Instroducción](#introduccion)
2. [Propósito](#proposito)
3. [Convenciones del documento](#Convenciones-del-documento)
4. [Público objetivo y sugerencias de lectura](#Público-objetivo-y-sugerencias-de-lectura)
5. [Definición del producto](#Definición-del-producto)



## 1. Introducción 
### 1.1 Propósito
El software descrito en este documento consiste de una aplicación para dar y tomar asesorías de manera institucional. Se busca que esta aplicación ayude a los alumnos a recibir asesorías de manera rápida y personalizada, además de proporcionar un espacio para aquellos alumnos que deseen brindar ayuda puedan hacerlo de manera segura y fácil.

Esta aplicación podrá utilizarse tanto en dispositivos móviles como tabletas y computadores a través de un buscador de internet.  
### 1.2 Convenciones del documento 
### 1.3 Público objetivo y sugerencias de lectura
Está documentación está principalmente dirigida a programadores y desarrolladores que tengan al menos un conocimiento básico de lenguajes como Python, HTML, C#, entre otros. Deben, además comprender el funcionamiento de las bases de datos y los servicios web. 
### 1.4 Definición del producto
Esta aplicación podrá beneficiar a todos los alumnos que estén buscando ayuda en sus materias a un bajo precio y con la seguridad de que, quien les ayudará, será alguien aprobado por los mismos profesores. Les permitirá buscar asesores específicos para cada materia y tema; podrán revisar las notas de dichos asesores para asegurarse de que la ayuda que reciben sí se acoplará a sus necesidades. 
La plataforma, además, representará un lugar seguro para que los asesores suban su material y puedan ser remunerados por éste.  
## 2. Descripción general 
### 2.1 Perspectiva del producto 
Este producto surge a partir de la necesidad de los alumnos del Instituto Tecnológico Autónomo de México (ITAM) de contar con una plataforma segura, a través de la cual puedan dar y recibir asesorías. Con esta plataforma, aquellos alumnos que deseen dar asesorías podrán anunciarse, especificar sus materias de interés y dar a conocer los horarios y los costos de sus asesorías. Principalmente se busca desarrollar una plataforma en la que se asegure a los alumnos que las asesorías que recibirán serán impartidas por otros alumnos aprobados por profesores.
### 2.2 Funcionalidades del producto 
Para los alumnos que busquen tomar alguna asesoría, la aplicación les permitirá
* buscar un asesor según la materia de interés 
* agendar una sesión con uno de los asesores disponibles 
* calificar al asesor 
* leer y descargar los documentos adicionales del asesor

Para los alumnos que deseen brindar asesorías a sus compañeros, la aplicación les permitirá: 
* solicitar su verificación como asesores 
* agregar una materia para la cual dar asesorías 
* eliminar una materia para la cual dio asesorías 
* subir archivos adicionales para complementar sus asesorías 

A través de la aplicación, los administradores podrán: 
* recibir la notificación para verificar a un alumno como asesor
* verificar o rechazar a un alumno como asesor
### 2.3 Clases de usuario 
Por un lado, tenemos a los alumnos que están buscando ser asesorados en alguna materia. Estos alumnos podrán tener acceso a la base de datos de asesores, podrán confirmar si los asesores están verificados por los profesores, y, además, podrán agendar asesorías con la persona que consideren que más se adapta a sus necesidades. 

Por otro lado, los asesores podrán solicitar ser verificados por los profesores para que, así, se les pueda remunerar su trabajo. Además, tendrán la posibilidad de subir apuntes, ejercicios o cualquier material de apoyo para sus asesorías. Nótese que ellos también tendrán todas las funcionalidades de los alumnos.
Finalmente, los profesores podrán revisar quiénes han solicitado su verificación como asesores, revisar sus notas y aprobarlos o rechazarlos. 
### 2.4 Entorno operativo 
La plataforma funcionará en cualquier buscador y en cualquier dispositivo (computadoras, celulares, tablets, etc.). No tendrá ninguna restricción en cuanto al entorno operativo. 
### 2.5 Restricciones de diseño e implementación 
El programa únicamente podrá ser utilizado por miembros de la comunidad del ITAM (alumnos y profesores), al menos en la fase inicial del software. De igual manera, el tamaño de los documentos que se podrán subir estará restringido a la capacidad de Google Drive, plataforma que se utilizará para almacenar todos los documentos. 
### 2.5 Documetnación del usuario 
### 2.6 Suposiciones y dependencias 
En este documento se asume que todos los usuarios tendrán una cuenta de Comunidad ITAM y un correo institucional.
## 3. Reuqisitos de la interfaz externa 
### 3.4 Interfaces de comunicaciones 
Todos los usuarios deberán permitir el acceso a sus cuentas de correo, a través de las cuales se enviarán las solicitudes de asesorías, o bien, se recibirán estas solicitudes. No se les pedirá ningún otro dato a los usuarios más que su nombre, correo y, en caso de así permitirlo, su número de teléfono. 
## 4. Características del sistema 
## 5. Otros reauisitos no funcionales 
### 5.1 Reglas de la plataforma 
1. Únicamente los profesores y los administradores de la plataforma podrán aprobar a los asesores. 
2. Los asesores podrán dar asesoría de cualquier materia que decidan, sin embargo, la remuneración que tendrán por éstas dependerá de si están aprobados o no para dichas materias. 
3. Los asesores, al igual que los usuarios normales, podrán solicitar asesorías de ciertas materias. 
## Apéndice A: Definición de la arquitectura 
Para este proyecto se utilizó una combinación de arquitectura por capas y arquitectura de microservicios. La decisión para utilizar capas se tomó basándonos en la experiencia de los desarrolladores, en su nivel de conocimientos y el tiempo con el que se contaba para desarrollar el proyecto. La arquitectura por capas es la más fácil de desarrollar y probar, pues no necesitaba que contáramos con un Senior Developer para utilizarla. Los microservicios fueron necesarios, pues en ellos se almacenarán los archivos que los usuarios carguen en la plataforma. 
## Apéndice B: Metodología de trabajo 
Utilizamos una metodología Feature Driven para desarrollar el proyecto, pues de esta forma varios integrantes del equipo pudieron trabajar en diferentes funcionalidades a la vez, sin que el trabajo de uno interfiriera con el otro. Además, así se pudo aprovechar de la mejor manera el tiempo con el que dispusimos. 
## Apéndice C: Casos de uso







