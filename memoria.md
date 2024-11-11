# Memoria de examen DAW

## Indice
[Introduccion](#introduccion)
[Resumen](#resumen)
[Realizacion de las actividades](#realización-de-las-actividades)
[Valoración de los resultados](#valoración-de-los-resultados)
[Conclusión](#conclusion)


## Introduccion
En esta memoria esta redactada la realización del examen de la primera avaluación de la asignatura DAW.
Se ha realizado mediante consola de comando de Ubuntu en el centro de estudios Diactica.
Utilizaremos Apache ssh y la consola de comandos para realizar este examen.

## Resumen
Primeramente Realizare el examen tipo test.
Posteriormente creare un archivo mediante ssh y linea de comando.
Finalmente creare una pagina web local con su host virtual.

## Realización de las actividades
### Ejercicio 1

He realizado el examen tipo test:
![ExamenDAW](https://github.com/user-attachments/assets/9ed87783-7b77-442c-8cf3-589fbf020023)


### Ejercicio 2

Primeramente he accedido a una maquina remota mediante ssh :

![conexion ssh](https://github.com/user-attachments/assets/ccf8677f-281c-4f8c-b074-5bff69e81543)

Posteriormente he creado en el escritorio un archivo txt con mi nombre y apellidos:

![CrearEnEscritorio](https://github.com/user-attachments/assets/e03c107a-e3ab-4a39-bbcf-74fdd49143f0)

Conteniendo, el resultado de whoami y el comando necesario para saber quién está conectado a la máquina mediante ssh (Who), dentro:

(El Who lo introduzco me diante el comando ***tee -a RamonVinuales.txt*** aunque tambien se podira introducir con un echo siendo:***echo "Who" >> RamonVinuales.txt***)  

![RamonVinualesTxt](https://github.com/user-attachments/assets/ad76f39a-614f-4310-bac7-bb5d819afb78)

### Ejercicio 3

Primero creo una pagina web sencilla en la ubicacion /var/www/miWeb de mi maquina, llamada index.html:
![CrearIndexHtml](https://github.com/user-attachments/assets/634a0c68-d6d0-442e-8ecb-891d1f06b545)
![indexHtml](https://github.com/user-attachments/assets/f5b216b3-6259-4745-894d-e18db3dbcb53)

Posteriormente creare un host virtual para poder llegar a esa pagina,copiando 000-default.conf y llamandola examenDaw.conf:

![cp](https://github.com/user-attachments/assets/8f4220a8-8e15-42ef-992a-15cb565b5b29)

Modificare esta examenDaw.conf para que funcione correctamente:

![entrarEnElConf](https://github.com/user-attachments/assets/7cf0276d-a327-4ae8-8734-35caa5111024)
![conf](https://github.com/user-attachments/assets/38570247-d19a-426e-aafe-8476c63d2cd5)

Posteriormente le hare un a2ensite al nuevo conf para que funcione correctamente:
![a2ensite](https://github.com/user-attachments/assets/f1a7345f-3be8-42a5-aa51-ef4dc26001fe)

Finalmente modificare /etc/hosts para añadir el nuevo dominio a la lista (Es la 5a linea : ***127.0.0.1 daw.ejercicio3.com***):
![hosts](https://github.com/user-attachments/assets/9c73ad6a-c3e6-4194-8b82-c32da54a31b7)
![ejercicioDaw](https://github.com/user-attachments/assets/a9dc0ddf-648f-4a26-bc48-2368b18c6501)

Por ultimo se lo he enseñado al profesor y me ha dado el visto bueno.

## Valoración de los resultados

He conseguido realizar correctamente el examen tal y como se pedia en el enunciado.

## Conclusion

Tras realizar el examen y ver que las cosas que pedia el enunciado me han salido correctamente puedo suponer que sacare buena nota en este examen

