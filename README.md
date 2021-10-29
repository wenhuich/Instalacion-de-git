# Instalacion-de-git

### Paso inicial:
Para comprobar si está instalado ya la aplicación poner el comando:
```
git version
```
Si no está, entonces puedes empezar con la instalación.

### Paso 1:
Para empezar a instalar tenemos que empezar con el siguiente comando:
```
sudo apt update
```
Poner su contraseña y darle a enter.

![1](https://user-images.githubusercontent.com/91631138/139467617-94510a79-28f0-4357-ac6d-fc178e7854b9.png)

### Paso 2:
Una vez que haya finalizado la instalación, empezamos con la instalación de Git:
```
sudo apt install git
```
Te pedirá que pongas si o no seguir con la actualización.

![2](https://user-images.githubusercontent.com/91631138/139467762-72f70a30-7caa-4e37-bbd0-b3d2177150b3.png)

### Paso 3:
Para verificar que se ha instalado correctamente, ejecutamos el siguiente comando:
```
git --version
```

![3](https://user-images.githubusercontent.com/91631138/139467847-6b021093-97af-4d5c-830d-5572c3a1a1c5.png)

### Paso 4:
Para actualizarlo a la versión más reciente, ejecutar el siguiente comando:
```
sudo apt update
sudo apt install libz-dev libssl-dev libcurl4-gnutls-dev libexpat1-dev gettext cmake gcc
```
Te pedirá que confirmes si o no.

![4](https://user-images.githubusercontent.com/91631138/139467969-1f3e5287-78f8-48eb-a3f1-e1d4bbaf7131.png)

### Paso 5:
Ahora tenemos que buscar la actualización más reciente o al que desee utilizar, primero ejecutamos este comando para que puedas poner el versión que quieres;
```
mkdir tmp
cd /tmp
```

![5](https://user-images.githubusercontent.com/91631138/139468039-1b2f5288-d18d-4f4e-aee2-7d3cb4eb93d3.png)

Para buscar el versión que quieres accedemos a esta página:
https://mirrors.edge.kernel.org/pub/software/scm/git/

### Paso 6:
Ahora ponemos este comando:
```
curl -o git.tar.gz https://mirrors.edge.kernel.org/pub/software/scm/git/git-2.29.3.tar.gz
```
Si os parece algo así, necesitáis descargar el curl.

![6](https://user-images.githubusercontent.com/91631138/139468258-0f6dbfef-24d9-46cf-bdac-552e6ef415e7.png)

Y le ponemos de nuevo el comando:
```
curl -o git.tar.gz https://mirrors.edge.kernel.org/pub/software/scm/git/git-2.29.3.tar.gz
```

![7](https://user-images.githubusercontent.com/91631138/139468367-00696cf5-be68-4cd7-8b34-56d5994dc66e.png)

### Paso 7:
Descomprimimos el archivo tarball con el siguiente comando:
Depende también de donde lo hayas descargado el archivo.
```
tar -zxf git.tar.gz
```
Tienes que ir al nuevo directorio con el siguiente comando:

![8](https://user-images.githubusercontent.com/91631138/139471722-e4637a0f-1a01-4055-a8fa-df6cf7090fc5.png)

```
 exec bash
```

### Paso 8:
Ahora, puedes crear el paquete e instalarlo escribiendo estos dos comandos:
```
make prefix=/usr/local all
```

![9](https://user-images.githubusercontent.com/91631138/139472027-1d9df741-1109-4219-948a-fda058d19012.png)

```
sudo make prefix=/usr/local install
```

![10](https://user-images.githubusercontent.com/91631138/139472169-9d80cd4a-98b3-45ab-bdfc-b57143c283fe.png)

### Paso 9:
Y ya lo tendríamos, sólo falta sustituir el paquete shell para que se utilice la versión de Git que acabamos de instalar:
```
 exec bash
 ```
 ### Paso 10:
comprobamos si ya está con el siguiente comando:
```
git --version
```
![11](https://user-images.githubusercontent.com/91631138/139472301-7c3b5006-ccd6-4a68-92e6-f9dfe6e2db11.png)

### Paso 11:
Ahora toca configurar tu Git.
Con este comando, tienes que poner tu nombre de tu github:
```
git config --global user.name "Your Name"
```
Y con este, tu correo:
```
git config --global user.email "youremail@domain.com"
```
Ahora para ver lo que se ha guardado:
```
git config --list
```
Y ya estaría.
 
 
 
 
 
 

