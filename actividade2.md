
# Guía Básica de Uso de VirtualBox

En esta guia técnica los conceptos fundamentales y los pasos necesarios para crear, configurar y gestionar máquinas virtuales con **VirtualBox**.

---

## INDICE
1. [Introducción](#1-introducción)
2. [Requisitos previos](#2-requisitos-previos)
3. [Procedimiento de uso](#3-procedimiento-de-uso)
   * [3.1 Creación de una nueva máquina virtual](#31-creación-de-una-nueva-máquina-virtual)
   * [3.2 Configuración del hardware virtual](#32-configuración-del-hardware-virtual)
   * [3.3 Instalación del sistema operativo](#33-instalación-del-sistema-operativo)
4. [Tipos de red en VirtualBox](#4-tipos-de-red-en-virtualbox)

---

## 1. Introducción

**VirtualBox** es un software gratuito y de código abierto que permite crear y ejecutar entornos virtualizados en un equipo anfitrión. Es una herramienta clave en informática para probar sistemas operativos, ejecutar software en entornos aislados y configurar servidores de prueba.

---

## 2. Requisitos previos

Antes de comenzar a trabajar con VirtualBox, asegúrate de contar con los siguientes elementos:

* **Equipo anfitrión:** Procesador *x86/x64* compatible con virtualización habilitada.
* **Memoria RAM:** Mínimo **8 GB** de memoria RAM instalada (para poder asignar al menos *2 GB o 4 GB* a la máquina virtual).
* **Almacenamiento libre:** Al menos **25 GB** de espacio libre en disco SSD/HDD.
* **Imagen ISO:** Archivo de imagen del sistema operativo que deseas instalar (por ejemplo, *Ubuntu Desktop* o *Debian*).
* **Software:** Descargar la última versión instalable desde el [Sitio Oficial de VirtualBox](https://www.virtualbox.org).

---

## 3. Procedimiento de uso

![Interfaz principal de Oracle VM VirtualBox](imagenes/virtualbox_gui.png)

### 3.1 Creación de una nueva máquina virtual

1. Abre la aplicación **VirtualBox** y haz clic en el botón **Nueva** (o utiliza el atajo `Ctrl + N`).
2. Introduce el **Nombre** identificativo de la máquina virtual (por ejemplo, *Ubuntu-2026*).
3. Selecciona la carpeta donde se almacenará la máquina virtual.
4. En el apartado **Imagen ISO**, examina tu equipo y selecciona el archivo `.iso` descargado.
5. Comprueba que el **Tipo** (*Linux*) y la **Versión** (*Ubuntu 64-bit*) se hayan detectado correctamente.

### 3.2 Configuración del hardware virtual

1. Asigna la **Memoria RAM** (mínimo *2048 MB* recomendado para sistemas de escritorio).
2. Asigna el número de **Procesadores (CPU)** (mínimo *2 núcleos*).
3. Selecciona la opción **Crear un disco duro virtual ahora**.
4. Elige el formato de disco **VDI (VirtualBox Disk Image)** y marca la opción de *reservado dinámicamente* con un tamaño de al menos **25 GB**.

### 3.3 Instalación del sistema operativo

1. Selecciona la máquina virtual en el panel izquierdo y haz clic en **Iniciar**.
2. Completa el proceso de instalación interactivo del sistema operativo.
3. Una vez finalizado, desmonta la imagen ISO desde el menú `Dispositivos` > `Unidades ópticas` para evitar arrancar de nuevo el instalador.

---

## 4. Tipos de red en VirtualBox

VirtualBox ofrece diferentes modos de red para conectar las máquinas virtuales con la red física o entre sí:

| Modo de Red | Descripción | Uso Recomendado |
| :--- | :--- | :--- |
| **NAT** | La MV se conecta a Internet compartiendo la dirección IP del equipo anfitrión. | Navegación por Internet y descargas básicas. |
| **Adaptador Puente** | La MV obtiene su propia dirección IP en la red local física del anfitrión. | Configuración de servidores web, SSH o servicios en red. |
| **Red Interna** | Crea una red privada aislada entre varias máquinas virtuales del mismo anfitrión. | Pruebas de redes, laboratorios de seguridad y routers virtuales. |

---

## 5. Referencias

* [Documentación oficial de VirtualBox](https://www.virtualbox.org/wiki/Documentation)
* [Manual de usuario de VirtualBox](https://www.virtualbox.org/manual/UserManual.html)