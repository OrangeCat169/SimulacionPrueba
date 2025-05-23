# SimulacionPrueba
***Este repositorio está hecho con el proposito de reforzar para la prueba de Patrones de diseño***
- **Nombre:** Fernando Maximiliano Castro Figueroa
- **Sección:** 1

## 1.Diagrama de Casos de Uso
**Error Detectado:**
- 1. El primer error detectado es que no aplica `<<Include>>` ni `<<Extend>>` en el diagrama proporcionado, o los usa de una forma erronea
- 2. El usuario puede eliminar el historial de las reservas
**Justificacion:**
- 1. la forma correcta de aplicar los `<<Include>>` seria con una linea interlineada y con el nombre encima(**----->**), tambien la forma de uso, es directamente al momento de un actor usar esa funcion siempre te llevará a la siguiente.
     y en cuanto a los `<<Extend>>` es con una linea interlineada apuntando hacia atras y con el nombre encima(**<-----**), y la forma de uso es, al momento de el acor realizar la accion puede o no usarse la siguiente.
- 2. El usuario no deberia poder eliminar las reservas de otras personas
**Correccion:**
- 1. las lineas mal imnplementadas dentro del diagrama, cambiarlas por lineas interlineadas que son las que realmente corresponden `<<Include>>` y `<<Extend>>`
- 2. El usuario no tiene acceso a eliminar el historial de reserva de otras personas, se elimina esa funcion

## 2.Diagrama de Clases
**Error Detectado:**
- 1. El usuario Puede hacer la reserva, pero nada le indica cuando hay (**Fecha**), ni si tiene disponibilidad (**estado**)
- 2. El usuario no agrega en ningun momento un numero de telefono como atributo para recibir notificacion como (**sms**)
- 3. La clase usuario no deberia llamarse como tal
**Justificacion:**
- 1. la clase reserva debe ir entre usuario y sala
- 2. para que el usuario pueda recibir un sms debe agregar como atributo un numero de telefono
- 3. ***USUARIO*** es todo aquel que usa el SW, incluido admins y super admins
**Correccion:**
- 1. cambiamos la clase de reserva entre usuario y y sala
- 2. dentro de la clase del usuario, agregamos el atributo **fono**
- 3. Cambiamos el nombre de la clase ***USUARIO*** a **CLIENTE** 

## 3.Diagrama de Implementacion
