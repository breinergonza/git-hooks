# Validar ortografía en español antes de hacer un commit "pre-commit"

## Uso:

Renombre el archivo "pre-commit.ValidarOrtografia" por "pre-commit" y agréguelo a la carpeta **.git/hooks/** 

Cada ves que realice un cambio el git hook hará una análisis de las palabras en los archivos modificados o creado que se van a subir al repositorio validando la ortografía a partir de un diccionario, en este caso, usara el diccionario de español para realizar la validación.

## Pre-condiciones:

Para que este git hook funcioné es necesario haber instalado **[`aspell`](http://aspell.net/)**. el cual es un corrector ortográfico gratuito y de código abierto.

Instalación con Homebrew para Mac o Windows:

	~]$ brew install aspell

Instalación en Ubuntu:

	~]$ apt-get install -y aspell

 o 

	~]$ sudo apt-get install aspell-es

Para validar en donde se encuentra instalado aspell se puede utilizar el comando:
```
which aspell
```