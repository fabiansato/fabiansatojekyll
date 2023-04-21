---
title: 'Git - Cheatsheet mas usados' 
date: '2022-12-02'
layout: post
tag: [tutorial, WebDev, Javascipt]
excerpt: >-
  El operador ternario es aquel que nos sirve para escribir el código de una sentencia if de una forma más sencilla. Veremos como hacerlo
description: >-
  El operador ternario es aquel que nos sirve para escribir el código de una sentencia if de una forma más sencilla. Veremos como hacerlo
image: '/images/blog/javascript-operadores-ternarios.webp'
thumb_image: '/images/blog/javascript-operadores-ternarios.webp'
style: code
author: fabiansato
---

## Introducción
El operador ternario es aquel que nos sirve para escribir el código de una sentencia if de una forma más sencilla. Imaginemos que tenemos un ejemplo que nos calcula cuál es el mayor de dos número en Javascript. El código sería sencillo como comprobamos a continuación.



## Configuracion
Descarga Para Mac OSX  windows y linux
https://git-scm.com/downloads

## crea un repositorio nuevo
Crea un directorio nuevo, ábrelo y ejecuta
`git init`
para crear un nuevo repositorio de git.

## Hacer checkout a un repositorio
Crea una copia local del repositorio ejecutando
`git clone /path/to/repository`
Si utilizas un servidor remoto, ejecuta
`git clone username@host:/path/to/repository`

## Flujo de trabajo

Tu repositorio local esta compuesto por tres "árboles" administrados por git.
El primero es tu **Directorio de trabajo** que contiene los archivos,
el segundo es el **Index** que actua como una zona intermedia, 
y el último es el **HEAD** que apunta al último commit realizado.

![fbb759f29fbba37b9ed52f9857962496.png](:/3ca795ef8653465f88f481b90306e5d1)

## add & commit
Puedes registrar cambios (añadirlos al Index) usando
`git add <filename>`
`git add .`
Este es el primer paso en el flujo de trabajo básico. Para hacer commit a estos cambios usa
`git commit -m "Commit message"`
Ahora el archivo esta incluído en el HEAD, pero aún no en tu repositorio remoto.

## Envio de cambios
Tus cambios están ahora en el `HEAD` de tu copia local. Para enviar estos cambios a tu repositorio remoto ejecuta
`git push origin master`
Reemplaza master por la rama a la que quieres enviar tus cambios.

Si no has clonado un repositorio ya existente y quieres conectar tu repositorio local a un repositorio remoto, usa
`git remote add origin <server>`
Ahora podrás subir tus cambios al repositorio remoto seleccionado.

# Ramas
Las ramas son utilizadas para desarrollar funcionalidades aisladas unas de otras. La rama master es la rama "por defecto" cuando creas un repositorio. Crea nuevas ramas durante el desarrollo y fusiónalas a la rama principal cuando termines.

![9f70f7f0ca42b8d88b14784f868e415b.png](:/2a2d9c52b9ed4c87a564d1476e186fbb)