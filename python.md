---
jupytext:
  text_representation:
    extension: .md
    format_name: myst
kernelspec:
  display_name: Python 3
  language: python
  name: python3
---
# Introducción a la programación en Python 
En la primera parte de estas prácticas usaremos el lenguaje de programación
Python. Para ello, nos valdremos de un entorno muy sencillo, los *Python
Notebooks*, que nos permiten programar en línea en entornos colaborativos
como [Google Colab](https://colab.research.google.com/).

## La terminal
Para usar el lenguaje de programación Python, tenemos una serie de opciones.
Una de ellas es usar la **línea de comandos** en una **terminal** de **Linux**.
La terminal es un programa que nos permite interactuar con nuestro ordenador, y
su aspecto es similar al de la figura que mostramos a continuación.

![terminal](https://upload.wikimedia.org/wikipedia/commons/2/29/Linux_command-line._Bash._GNOME_Terminal._screenshot.png)

Es importante conocer unos cuantos comandos de para navegar por nuestro sistema
operativo, listar el contenido de un directorio o copiar o eliminar archivos.
A continuación mostramos algunos de ellos:
* Comandos de Navegación y Exploración del Sistema:
    - `pwd`: Muestra el directorio actual (Print Working Directory).
    - `ls`: Lista los archivos y directorios del directorio actual.
    - `ls -l`: Lista con detalles adicionales (permisos, propietario, tamaño, etc.).
    - `cd [directorio]`: Cambia al directorio especificado.
    - `cd ..`: Sube un nivel en el árbol de directorios.
* Gestión de Archivos y Directorios
	- `touch [archivo]`: Crea un archivo vacío.
	- `mkdir [directorio]`: Crea un nuevo directorio.
	- `cp [origen] [destino]`: Copia archivos o directorios.
	- `mv [origen] [destino]`: Mueve o renombra archivos o directorios.
	- `rm [archivo]`: Elimina un archivo.
	- `rm -r [directorio]`: Elimina un directorio recursivamente.
	- `locate [archivo]`: Busca un archivo en el sistema.
* Visualización y Edición de Archivos
	-  `cat [archivo]`: Muestra el contenido de un archivo.
	-  `more [archivo]`: Permite visualizar un archivo de forma paginada.
	-  `head -n [número] [archivo]`: Muestra las primeras n líneas.
	-  `tail [archivo]`: Muestra las últimas líneas de un archivo.
	-  `nano [archivo]`: Abre un editor de texto sencillo.
	-  `vim [archivo]`: Abre un editor de texto avanzado.

Todos estos comandos son extremadamente útiles para que nos podamos mover
en nuestro **filesystem**, un árbol de directorios y archivos con un aspecto
como el del diagrama que mostramos a continuación, 

![filesystem](https://raw.githubusercontent.com/swcarpentry/shell-novice/refs/heads/main/episodes/fig/filesystem.svg)

## Python como calculadora
Python es tanto un lenguaje de programación como un lenguaje de *scripting*.
Al contrario de muchos otros lenguajes de programación, para ejecutar una
serie de directivas, tan sólo tenemos que escribirlas en un intérprete de Python.
Por ejemplo podemos usar Python para remplazar nuestra calculadora
```{code-cell} python
3 + 5 * 4
```

## Corriendo programas en Python
Para ejecutar código en Python, disponemos de múltiples 
opciones. En primer lugar, podemos escribir un programa
en un editor de texto y ejecutarlo desde la terminal. 
Este programa (llamado `hola_mundo.py`) podría ser tan`sencillo como el siguiente:
```python
#!/usr/bin/env python
# Our first Python program
print ("¡Hola mundo!")
```
En la terminal, luego tendríamos que escribir lo siguiente:
```bash
foo@bar:~$ python hola_mundo.py
```
También podemos correr el programa en una terminal de
Python, tecleando `python` o `ipython` en nuestra
terminal.
```shell
foo@bar:~$ python
Python 3.9.16 | packaged by conda-forge | (main, Feb  1 2023, 21:42:20)
[Clang 14.0.6 ] on darwin
Type "help", "copyright", "credits" or "license" for more information.
>>>
```
Finalmente, podríamos usar, como haremos en estas 
prácticas, un Jupyter Notebook. Los notebooks son 
interfaces gráficas a IPython que permiten combinar
celdas de código y de texto.

![jupyter](https://jupyter-notebook.readthedocs.io/en/latest/_images/notebook-running-code.png)

Python es un lenguaje de programación enormemente potente, que 
maximiza la legibilidad del código, por lo que es ideal para introducirse
en el mundo de la programación.

![python-flying](https://imgs.xkcd.com/comics/python.png)