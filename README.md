# Game Project

Para correre el juego debes seguir las siguientes instrucciones en la terminal:

```sh
cd game
python3 main.py
```

# App Project

```sh
git clone
cd app
python3 -m venv env
source env/bin/activate
pip3 install -r requirements.txt
python3 main.py
```

#### Comandos Utilizados
- python
- python3
- exit() para salir de la interfaz de python

#### Instalación
- apt update
- sudo apt update
- sudo apt -y upgrade

#### Verificar Instalación de python
- python3 -V

#### Instalación de gestor de paquetes de dependencias
- sudo apt insstall -y python3-pip

#### Verificar Instalación del gestor
- pip3 -V

#### Dependencias en entorno profesional
- •	apt install -y build-essential libssl-dev libffi-dev python3-dev

### Crear repositorio en GITGUB
#### Comando para enlazar e inicializar
•	git init
•	git remote add origin (enlace gitgub)
•	git remote -v
•	git add *
•	git commit -m “Mi primer archivo”
•	git push origin master

Refrescar pagina y revisar
Despues de tener los dos archivos .gitignore y README.md_ agregarlo al gitgub, revisar que esten los tres archivos cargados.
**Enlace a pypi**
https://pypi.org/
#### Correr en la terminal los siguientes comandos
•	pip3 -V
•	ll
•	mkdir charts
•	cd charts/
#### Estando en la carpeta vamos a instalar un paquete
•	pip3 install matplotlib
Ver librerias instaladas
•	pip3 freeze
    import matplotlib.pyplot as plt
    
    def generate_pie_chart():
        labels = ['A', 'B', 'C']
        values = [200, 34, 120]
    
        fig, ax = plt.subplots()
        ax.pie(values, labels=labels)
        plt.savefig('pie.png')
        plt.close()
    import charts
    
    def run():
        charts.generate_pie_chart()
    
    if __name__ == '__main__':
        run()
#### Verificar donde esta python y pip
•	which python3
•	which pip3
#### Si estas en linux o wsl debes instalar
•	sudo apt install -y python3-venv
#### Poner cada proyecto en su propio ambiente, entrar en cada carpeta.
•	python3 -m venv env
#### Activar el ambiente
•	source env/bin/activate
#### Salir del ambiente virtual
•	deactivate
#### Podemos instalar las librerias necesarias en el ambiente virtual como por ejemplo
•	pip3 install matplotlib==3.5.0
#### Verificar las instalaciones
•	pip3 freeze

**Requirements.txt** = Archivo que gestiona todas las dependencias y en que versiones se necesitan.
#### Generar el archivo con el siguiente comando
•	pip3 freeze > requirements.txt
#### Revisar lo que hay dentro del archivo
•	cat requirements.txt
#### Instalar las dependencias necesarias para contribuir más rápido en proyectos
•	pip3 install -r requirements.txt
#### Preparar archivo para contribución
### #App Project
```sh
git clone
cd app
python3 -m venv env
source env/bin/activate
pip3 install -r requirements.txt
python3 main.py
#### Y luego subir los cambios a Gitgub
Llega luego el profe Juan DC 😃 JAJAJJAJAJA para hacer una Hermosa Contribución.

##### •	Crear un entorno
python3 -m venv env
##### •	Activar un entorno virtual
source env/bin/activate
##### •	Verificar que estemos dentro del entorno virtual
which python3
##### •	Instalar la dependencia dentro del entorno virtual
pip3 install requests
##### •	Verificar la instalacion
pip3 freeze
##### •	Crear el archivo para que cualquier persona pueda desplegar el proyecto
pip freeze > requeriments.txt
### STORE
    import requests
    
    def get_categories():
        r = requests.get('https://api.escuelajs.co/api/v1/categories')
        print(r.status_code)
        print(r.text)
        print(type(r.text))
        categories = r.json()
        for category in categories:
            print(category['name'])
    MAIN
    import store
    
    def run():
        store.get_categories()
    
    if __name__ == '__main__':
        run()

### PANDAS
•	Es una de las librerias mas utilizadas en python y nos sirven para analizar y manipular datos de archivos duros
##### Activar anbiente del proyecto
source env/bin/activate
##### Verificar
which python3
##### Ver que hay dentro del archivo en el cual se evidencia que no hay pandas
cat reqruirements.txt
##### Agregar nueva libreria
pip3 install pandas
##### Verificar librerias instaladas
pip3 freeze
##### Actualizar el documento que contiene las librerias
pip3 freeze > requirements.txt
