# Nginx-server
## Instalación y configuración del servidor web Nginx: Virtual Hosts

### El primer paso es instalar nginx.
![image](https://user-images.githubusercontent.com/91564971/167221079-7f5bc769-cc4a-4be7-b2d4-199aaeb48f09.png)

### Luego para ver si todo está instalado y correcto revisaremos el estado de nginx.
![image](https://user-images.githubusercontent.com/91564971/167221268-583105e1-0f0b-4fd3-a899-1e32498486da.png)

### Por si acaso comprobaremos si todo esta correcto escribiendo en nuestra barra del buscador pondremos 'localhost'.
![image](https://user-images.githubusercontent.com/91564971/167221470-688a76f9-db6b-492d-ac2f-3122b921d439.png)

### Nos dirigimos a la carpeta de nginx y ejecutamos el comando 'ls' para ver una lista de carpetas contenidas en nginx.
![image](https://user-images.githubusercontent.com/91564971/167221883-8eb879f9-24e5-4ea5-814e-63d993fb48cd.png)

### Luego nos dirijimos a la carpeta index.html y entramos con el comando 'sudo vim'
![image](https://user-images.githubusercontent.com/91564971/167222138-32b665a5-afe3-42a9-acba-f8070f44db5b.png)

### Una vez dentro del index.html veremos la configuración del servidor que viene por defecto
![image](https://user-images.githubusercontent.com/91564971/167222209-ff15f953-0976-42a2-9201-4759581437ae.png)

### Con esto ahora pasamos a crear los 2 subdominios y para empezar creamos dos carpetas que contendrán el código html.
![image](https://user-images.githubusercontent.com/91564971/167222694-335ff330-e85b-452e-84f8-b15ae6d608c7.png)

### Copiamos el html con el mismo nombre en dichas carpetas creadas previamente con el comando 'cp'.
![image](https://user-images.githubusercontent.com/91564971/167222809-29db8a12-b0dd-4958-a574-51669d6a6ba2.png)

### Luego nos dirijimos en la carpeta de 'sites-available' y creamos dos servidores mas copiandolo del que viene por defecto.
![image](https://user-images.githubusercontent.com/91564971/167223366-a66a55dd-a54a-4014-8d40-53ea8404d01d.png)

### Nos metenos dentro y lo editamos con el comando 'sudo vim' y una vez dentro debemos canviarle 3 cosas: quitarle el default server ya que solo puede haber una, cambiar la ruta de root por la que hemos creado previamente y por ultimo ponerle nombre al servidor.
![image](https://user-images.githubusercontent.com/91564971/167223542-546a4420-0411-4fe8-86a6-d6e7e19f2d43.png)

### Repetir el proceso con el otro subdominio.
![image](https://user-images.githubusercontent.com/91564971/167223577-d27e3743-bd37-48d8-bbd7-04eea966f85e.png)

### Ahora vamos la carpeta de hosts y editamos hosts poniendo la ip del los otros 2 subdominios poniendo '127.0.1.1' y el nombre.
![image](https://user-images.githubusercontent.com/91564971/167223680-239cb999-d24e-4b4a-9584-91ef224d3f24.png)

### Luego con el comando 'sudo nginx -s reload' guardamos y reiniciamos los ajustes de nginx.
![image](https://user-images.githubusercontent.com/91564971/167223696-5292e24f-3f7a-450d-86bd-de446cbc9d40.png)

### Por último comprobamos si todo ha ido como toca y ponemos en la barra de nuestro navegador los nombres que hemos elegido.
![image](https://user-images.githubusercontent.com/91564971/167223798-f7573cda-d391-4203-8a45-c810bda54e52.png)
![image](https://user-images.githubusercontent.com/91564971/167223811-e74ea7c9-4434-4534-ba55-873221bcc218.png)

