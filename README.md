# termux-angular-config


Configuración de [Termux](http://termux.com/) [App](https://play.google.com/store/apps/details?id=com.termux) para generar un entorno de programación Angular sobre Android.


Luego de instalarte Termux, copia el siguiente comando y ejecútalo en su terminal:


```bash
apt update ; \
apt install -y wget ; \
hash -r ; \
wget -qO- https://github.com/andrescenci/termux-angular-config/raw/master/scripts/setup.sh | bash -x ; \
source ~/.bashrc
```


Esto es el contenido del script [start.sh](scripts/start.sh).


Este comando bajará y ejecutará este script del repositorio [setup](scripts/setup.sh).

Cuando todo finaliza solo nos resta crear un proyecto Angular, entonces ejecutamos:

```bash
ng new myApp
```

Y al finalizar la creación del proyecto, ejecutamos:

```bash
cd myApp
ng serve 
```

Y listo, el proyecto ya se encuentra levantado. Lo podemos ver en funcionamiento abriendo el browser del dispositivo en localhost:4200

Mas info sobre la instalación y los plugins utilizados con Vim en [Medium](https://medium.com/@andrescenci/angular-sobre-android-c023a6138d37).

