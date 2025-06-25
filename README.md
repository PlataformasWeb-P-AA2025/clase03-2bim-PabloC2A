# clase03-2bim

![img.png](img.png)
1️⃣ Desde cada estudiante
📌 ¿Cómo funciona?
mis_numeros_telefonicos es el related_name definido en el modelo NumeroTelefonico, lo que permite acceder a los números telefónicos de cada estudiante directamente.

2️⃣ Desde la consulta general
📌 ¿Cómo funciona?
mis_numeros_telefonicos es una lista independiente que contiene todos los números telefónicos de la base de datos.

### 25 junio 2025
El formulario hereda de ModelForm y personaliza su constructor __init__ para recibir explícitamente un objeto estudiante, 
el cual se asigna al diccionario initial del formulario para predefinir el valor de ese campo, luego se configura su widget 
como HiddenInput para ocultarlo de la vista del usuario, garantizando así que, al procesar el formulario con form.save(), 
el objeto NumeroTelefonico resultante ya esté vinculado correctamente al estudiante sin intervención del usuario.
