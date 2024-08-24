# El uso basico de PIP 

PIP es un administrador de paquetes que viene con Python desde la version 2.7.9 (o superior)

si quieres saber que version de python tienes, utiliza el comando en powerhell o bash

```sh
python --version
```

****

1. Instalacion de Paquetes

```sh
pip install [paquete]
```

2. Listar Paquetes Instalados
```sh
pip list
```
```sh
pip freeze
```

3. Generar un .txt con los paquetes instalados 
(Esto sirve si otra persona quiere tu codigo solo tendra que instalar tos paquetes de la lista de paquetes)
```sh
pip freeze > requirements.txt
```

4. Instalar paquetes de un .txt
```sh
pip install -r requirements.txt
```
```sh
pip install -r .\requeriments.txt
```