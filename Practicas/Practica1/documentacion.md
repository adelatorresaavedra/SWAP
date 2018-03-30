Primer paso : Instalar apache2 mysql-server y mysql-client, aquí surge un problema que se soluciona actualizando la máquina con apt-get update, procedo a instalar que antes no se ha podido instalar.

imágenes: 1_paso, 1_error, update , 1_instalaciónCompleta


Segundo paso: Comprobamos la versión  del servidor con apache2 -v y para ver si está en ejecución usamos la orden ps aux | grep apache

imágenes: 2.1_paso, 2.2_paso, 2.3_paso


Tercer paso: instalamos curl con apt-get install curl y nos vamos a la ruta con cd /var/www y creamos con nano un documento html con la información que nos pide en la práctica

imágenes : 3.1_paso, 

Cuarto paso: vamos a la segunda máquina le instalamos todo e intento que reciba el documento, no lo recibe y compruebo que se están viendo con ping "IP", efectivamente, se están viendo, 

imágenes: 4_error

Quinto paso : voy a la maquina 1 y modifico el documento por si falla algo. Rehago el documento voy a la máquina 2 y paso la orden curl, todo funciona perfectamente.

imágenes: 5_solucion

Sexto paso: Instalar ssh, con apt-get install ssh, miramos la ip de la máquina virtual 2 y escribimos la orden ssh “IP”, ahora estamos conectados remotamente a la máquina 2

imágenes: ssh1, ssh2 

