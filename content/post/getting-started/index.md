---
authors:
- admin
- Gabriel Corrales Jiménez
- 吳恩達
categories:
- Demo
- 教程
date: "2021-09-07T00:00:00Z"
draft: false
featured: true
lastmod: "2021-09-07T00:00:00Z"
projects: []
subtitle: "Capacidades que ofrecen las bases de datos espaciales para la implementación de flujos de trabajo en entornos multiusuario."
summary: "En este trabajo se realiza una introducción a la edición de bases de datos espaciales, haciendo una diferenciación entre la edición versionada y la no versionada. Específicamente se desarrollan dos flujos de trabajo sencillos de edición multiusuarios no versionada utilizando PostgreSQL en combinación con QGIS, y por otra parte ArcGIS, de manera que el lector pueda tener una visión."
tags:
- Academic
- 开源
title: FLUJOS DE TRABAJO EN BASES DE DATOS MULTIUSUARIO 
---

## Edicion multiusuario

Los SIG (*sistemas de información geográfica*) son sistemas integradores de tecnología informática, personas e información geográfica para capturar, analizar, almacenar y representar datos georreferenciados.

Al ser el almacenamiento parte fundamental de los SIG, las bases de datos juegan un papel muy importante en estos sistemas, de ahí que la mayoría de los actuales SGBD (*Sistemas Gestores de Bases de Datos*) permitan la incorporación de información geográfica. **De esta manera se originan las bases de datos espaciales**, para almacenar entidades del mundo real que ocupan un lugar en el espacio y mantienen relaciones espaciales entre ellas y el resto de elementos del entorno.

Son las bases de datos espaciales las que permiten la edición de estos elementos en entornos de trabajo multiusuario. La edición multiusuario se puede llevar a cabo de dos formas, la **edición no versionada**, que realiza ediciones y actualizaciones dinámicas de las capas sin la utilización de diferentes versiones de las tablas. Esta metodología se puede llevar a cabo mediante el uso de vistas, que son tablas virtuales que almacenan consultas como objetos, pero que en realidad sólo almacenan su definición y no los datos propiamente.

**La edición versionada**, por su parte, trabaja en diferentes versiones, aislando el trabajo en diferentes sesiones de edición que permiten la edición concurrente. Este método conserva una versión principal original o versión predeterminada.

La edición versionada es la forma más robusta de trabajo multiusuario. Requiere de una conexión con una base de datos relacional como *IBM DB2*, *Informix*, *Oracle*, *PostgreSQL* o *Microsoft SQL Server*, así como un administrador de bases de datos involucrado en el proceso, por lo que es el método más complicado de establecer.

## Más sobre este tema:

-  💡 {{< icon name="download" pack="fas" >}} Descarga nuestro {{< staticref "uploads/Articulo_ALGF_GCJ.pdf" "newtab" >}}artículo{{< /staticref >}}.

- Conoce más sobre las **[Bases de datos Multiusuario](https://www.cursosgis.com/almacene-sus-datos-espaciales-en-un-sistema-de-gestion-de-bases-de-datos-relacionales-sgbdr/)** aquí. 

