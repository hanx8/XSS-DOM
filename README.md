En el ejercicio XSS DOM de DVWA, se tiene el código inicial(XSS-DOM-INICIAL.txt)


Cómo se muestra en XSS DOM, se inserta el script:


127.0.0.1/a/vulnerabilities/xss_d/?default=English>/option></select><body onload=alert(“XSS”)>
  
  
El atacante intentará una técnica diferente para explotar la vulnerabilidad, puede insertar un script malicioso utilizando la función de carga de JavaScript> <body onload = alert ("XSS")> y enviar un enlace a la víctima. En este nivel, el atacante primero debe romper el bloque de selección para inyectar la carga del cuerpo o la etiqueta de imagen.
  
 
