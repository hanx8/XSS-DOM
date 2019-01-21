En el ejercicio XSS DOM de DVWA, se tiene el código inicial(XSS-DOM-INICIAL.txt)


Cómo se muestra en XSS DOM, se inserta el script:


127.0.0.1/a/vulnerabilities/xss_d/?default=English>/option></select><body onload=alert(“XSS”)>
  
  
El atacante intentará una técnica diferente para explotar la vulnerabilidad, puede insertar un script malicioso utilizando la función de carga de JavaScript> <body onload = alert ("XSS")> y enviar un enlace a la víctima. En este nivel, el atacante primero debe romper el bloque de selección para inyectar la carga del cuerpo o la etiqueta de imagen.
  
 
![image](https://user-images.githubusercontent.com/46895869/51500056-ae6c1a00-1d9a-11e9-91f0-c80ad12f53a9.png)


Para evitar que se inserte script, se crea una lista blanca de los lenguajes disponibles:

![image](https://user-images.githubusercontent.com/46895869/51500097-d8254100-1d9a-11e9-9e31-2a7221f84ab7.png)


Luego al realizar la misma prueba que se realizó al inicio, ya no se inserta el script:
