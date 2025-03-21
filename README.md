# Cliente Argentum Online Libre
![AO Logo](https://ao-libre.github.io/ao-website/assets/images/logo.png)

## Wiki Desarrollo Argentum Online
[Manual para entender el codigo de Argentum Online](http://es.dao.wikia.com/wiki/Wiki_Desarrollo_Argentum_Online).


## F.A.Q:

#### Error - Al abrir el proyecto en Visual Basic 6 no puede cargar todas las dependencias:
Este es un error comun que les suele pasar a varias personas, esto es debido que el EOL del archivo esta corrupto.
Visual Basic 6 lee el .vbp en CLRF, hay varias formas de solucionarlo:

Opcion a:
Con Notepad++ cambiar el EOL del archivo a CLRF

Opcion b:
Abrir un editor de texto y reemplazar todos los `'\n'` por `'\r\n'`

## Autoupdates:

El programa al iniciar comparara la version del programa que se encuentra en `INIT/Config.ini` en el parámetro [version](https://github.com/ao-libre/ao-cliente/blob/master/INIT/Config.ini) con la ultima version que se encuentra en el [Endpoint Github Releases](https://api.github.com/repos/ao-libre/ao-cliente/releases/latest). En caso de ser diferente, se ejecuta nuestro programa `ao-autoupdate` para poder hacer el update.

Para mas información sobre este proceso:

[Funcion para comparar versiones](https://github.com/ao-libre/ao-cliente/blob/master/CODIGO/frmCargando.frm#L121)

[Codigo fuente ao-autoupdate](https://github.com/ao-libre/ao-autoupdate)

## Revisar/Probar Pull Requests:
En caso que se quiera probar un PULL REQUEST hay que estar en el branch `master` y luego hacer un pull del Pull Request de la siguiente manera: `git pull origin pull/135/head` donde 135 es el numero de Pull Request

## Como hacer un release?
Aqui se deja explicado como hacer un release para cualquiera de las aplicaciones de Argentum Online Libre 
https://github.com/ao-libre/ao-cliente/wiki/How-to-create-and-publish-Releases%3F

## Documentacion oficial Visual Basic 6
While the Visual Basic 6.0 IDE is no longer supported, Microsoft's goal is that Visual Basic 6.0 applications continue to run on supported Windows versions. The resources available from this page should help you as you maintain existing applications, and as you migrate your functionality to .NET.

https://docs.microsoft.com/en-us/previous-versions/visualstudio/visual-basic-6/visual-basic-6.0-documentation

--------------------------

We start our branch from this version / old code:
* http://www.gs-zone.org/temas/cliente-y-servidor-13-3-dx8-v1.95611/




