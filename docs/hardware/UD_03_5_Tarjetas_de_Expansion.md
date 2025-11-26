---
title: 'UD 03.5 - Tarjetas de expansión GPY'
description: 'Apuntes sobre tarjetas de expansión, tipos y características.'
---


# UD 03.5 - Apuntes - Tarjetas de expansión

[Imprimir el Libro Completo](https://aules.edu.gva.es/fp/mod/book/tool/print/index.php?id=9389203#)

# UD 03.5 - Apuntes - Tarjetas de expansión

| Sitio: | AULES |
| --- | --- |
| Curso: | Sistemes informàtics-1CFSN |
| Libro: | UD 03.5 - Apuntes - Tarjetas de expansión |

| Imprimido por: | SERGIO REY MARTINEZ |
| --- | --- |
| Día: | miércoles, 22 de octubre de 2025, 16:50 |

## Tabla de contenidos

- [1. Introducción](https://aules.edu.gva.es/fp/mod/book/tool/print/index.php?id=9389203#ch56358)

- [2. Slot de expansión](https://aules.edu.gva.es/fp/mod/book/tool/print/index.php?id=9389203#ch56348)

- [3. Tarjetas gráficas](https://aules.edu.gva.es/fp/mod/book/tool/print/index.php?id=9389203#ch56349)

    - [3.1. Componentes](https://aules.edu.gva.es/fp/mod/book/tool/print/index.php?id=9389203#ch56344)

    - [3.2. GPU y Arquitectura](https://aules.edu.gva.es/fp/mod/book/tool/print/index.php?id=9389203#ch56361)

    - [3.3. Interfaces con placa base](https://aules.edu.gva.es/fp/mod/book/tool/print/index.php?id=9389203#ch56351)

    - [3.4. Salidas/conectores de la tarjeta gráfica](https://aules.edu.gva.es/fp/mod/book/tool/print/index.php?id=9389203#ch56345)

    - [3.5. Tarjetas gráficas integradas y dedicadas](https://aules.edu.gva.es/fp/mod/book/tool/print/index.php?id=9389203#ch56347)

    - [3.6. SLI/Crossfire](https://aules.edu.gva.es/fp/mod/book/tool/print/index.php?id=9389203#ch56363)

    - [3.7. Refrigeracíon](https://aules.edu.gva.es/fp/mod/book/tool/print/index.php?id=9389203#ch56362)

    - [3.8. Alimentación](https://aules.edu.gva.es/fp/mod/book/tool/print/index.php?id=9389203#ch56346)

    - [3.9. Multimonitor](https://aules.edu.gva.es/fp/mod/book/tool/print/index.php?id=9389203#ch56352)

  

- [4. Tarjetas de red](https://aules.edu.gva.es/fp/mod/book/tool/print/index.php?id=9389203#ch56343)

    - [4.1. Tarjeta para redes cableadas](https://aules.edu.gva.es/fp/mod/book/tool/print/index.php?id=9389203#ch56354)

    - [4.2. Tarjeta para redes Wifi](https://aules.edu.gva.es/fp/mod/book/tool/print/index.php?id=9389203#ch56355)

  

- [5. Tarjeta de sonido](https://aules.edu.gva.es/fp/mod/book/tool/print/index.php?id=9389203#ch56342)

    - [5.1. Canales y polifonia](https://aules.edu.gva.es/fp/mod/book/tool/print/index.php?id=9389203#ch56359)

    - [5.2. Operaciones básicas](https://aules.edu.gva.es/fp/mod/book/tool/print/index.php?id=9389203#ch56360)

    - [5.3. Componentes](https://aules.edu.gva.es/fp/mod/book/tool/print/index.php?id=9389203#ch56353)

    - [5.4. Salidas](https://aules.edu.gva.es/fp/mod/book/tool/print/index.php?id=9389203#ch56350)

  

- [6. Tarjetas de interfaz](https://aules.edu.gva.es/fp/mod/book/tool/print/index.php?id=9389203#ch56356)

- [7. Tarjetas capturadoras de vídeo](https://aules.edu.gva.es/fp/mod/book/tool/print/index.php?id=9389203#ch56357)

## 1. Introducción

Las tarjetas de expansión se insertan en las ranuras de expansión y permiten  mejorar y añadir nuevas funciones al equipo. Su misión es comunicar dispositivos periféricos internos como externos con el sistema de bus del ordenador.

Principalmente son

**VESA, PCI**

,

**AGP**

(todas estas prácticamente obsoletas) y

**PCI Express**

, y se instalan en el

**slot**

correspondiente.

Una vez insertadas en el ordenador, será necesaria su configuración en el sistema operativo mediante controladores o

*drivers*

y la instalación del software del fabricante. También existen tarjetas

*plug-and-pla*

y, que se configuran automáticamente con ayuda del sistema operativo.

Tarjetas de expansión más comunes:

- Tarjeta gráfica.

- Tarjeta de red: LAN o Wi-Fi.

- Tarjetas multimedia: sonido, captura de vídeo, captura de televisión, etc.

Además, es posible ampliar nuestro equipo con otras tarjetas como:

- Tarjetas de módem.

- Tarjetas de puertos USB.

- Tarjetas de puertos en serie o paralelo.

- Tarjetas controladoras de discos.

- Otras tarjetas adaptadoras; firewire, entradas/salidas, especificas de dispositivos, etc...

Debido al avance en la tecnología

*USB*

y a la

*integración de audio/vídeo en la placa base*

, hoy en día las tarjetas de expansión se emplean cada vez con menos frecuencia, integrándose en estos dispositivos todas las funcionalidades de las tarjetas de expansión convencionales.

<figure markdown="span" align="center">
  ![Imagen](./imgs/expansion/imagen.png){ width="85%" }
  <figcaption>Imagen</figcaption>
</figure>

Ejemplos de tarjetas:

## 2. Slot de expansión

Los Slots son unas ranuras de expansión de la placa base donde se insertan las tarjetas.

Incorporan cirucitos integrados para operar con diferentes periféricos o ampliar funcionalidades de un equpo

Los Slots pincipales son:

### PCI (PERIPHERAL COMPONENTS INTERCONNECT)

- Ancho de bus de 32 bits o 64 bits (33 MHz)

- Tasa de transferencia máxima de 133 MB por segundo en el bus de 32 bits (33,33 MHz × 32 bits ÷ 8 bits / byte = 133 MB / s)

- Tasa de transferencia máxima de 266 MB / s en el bus de 64 bits

- 3,3 V o 5 V, dependiendo del dispositivo

<figure markdown="span" align="center">
  ![Imagen](./imgs/expansion/imagen (2).png){ width="85%" }
  <figcaption>Imagen</figcaption>
</figure>

### AGP (ACCELERATED GRAPHICS PORT)

Uso exclusivo tarjetas gráficas. En desuso.

- **Versión 4x**

  , tasa de transferencia máxima de 1 GB / s (266 MHz × 32 bits ÷ 8 bits / byte = 1.064 MB / s)

- **Versión 8x**

  , tasa de transferencia máxima de 1 GB / s (533 MHz × 32 bits ÷ 8 bits / byte = 2.132 MB / s

- Tensiones:

<figure markdown="span" align="center">
  ![Imagen](./imgs/expansion/imagen (3).png){ width="85%" }
  <figcaption>Imagen</figcaption>
</figure>

### PCI EXPRESS (PCI-E)

PCI Express (Peripheral Component Interconnect Express) es un bus seriado de datos de alta velocidad. Cuya función es la de comunicar entre sí los diferentes componentes de hardware de un PC. Estos componentes pueden tener todos sus controladores en la placa base. O bien pueden usar controladores externos, en el caso de tratarse de tarjetas de expansión.

Este bus comenzó a introducirse en el año 2003. Y se desarrolló como sustituto del, ya extinto, bus PCI que empleaban las placas base hasta ese momento.

##### Versiones del bus PCIe desde su creación

Actualmente, se han desarrollado 6 versiones diferentes del bus PCIe:

- **PCIe 1.0**

  : presentado en el año 2003, tenía una capacidad de transferencia de datos de 2,5 GT/s (GigaTransfers por segundo) y de 250 MB/s por cada vía de datos.

- **PCIe 2.0**

  : del año 2007, doblaba la tasa de transferencia de datos a 5 GT/s y a 500 MB/s por cada vía de datos.

- **PCIe 3.0**

  : del año 2010, volvía a doblar las tasas de transferencia de archivos hasta los 8 GT/s y 984,6 MB/s por vía de datos. Precisamente por ello nunca hubo gran diferencia de rendimiento entre usar una tarjeta gráfica para este bus, en un bus PCIe 2.0.

- **PCIe 4.0:**

  del año 2017, vuelve a doblar las tasas de transferencia hasta los 16 GT/s y 1.969 MB/s. Este bus de datos ha comenzado a verse recientemente en las placas base para los procesadores AMD Ryzen 3000 y Threadripper 3.

- **PCIe 5.0**

  : su especificación se ha finalizó el año pasadoe año. Y, como es habitual, vuelve a doblar los datos de la anterior especificación hasta los 32 GT/S y 3.938 MB/s.

- **PCIe 6.0**

  : su especificación todavía no está finalizada (se la espera para el final del año 2021). Pero volverá a doblar las especificaciones anteriores, llegando hasta los 64 GT/s y 7.8777 MB/s por cada vía de datos.

Una particularidad del bus PCIe, es que es un bus modular. Es decir, que
 los conectores que se emplean en la placa base, no tienen todos las 
mismas características. En función del número de vías de datos PCI 
Express conectada a ellos, pueden ser conocidos como x1, x4, x8 o x 16.

Esto
 quiere decir que físicamente cada conector tiene un número de pines de 
contacto determinado, donde por ejemplo el conector de mayor tamaño, el 
x16, puede tener todos los contactos habilitados en su longitud, o en 
cambio tener solo la mitad, lo que rebajaría su velocidad a x8 
lógicamente.

<figure markdown="span" align="center">
  ![Imagen](./imgs/expansion/imagen (6).png){ width="85%" }
  <figcaption>Imagen</figcaption>
</figure>

### Factor de forma y tarjetas de expansión

Las tarjetas de expansión vienen preparadas para los diferentes factores de forma de las cajas de los equipos:

<figure markdown="span" align="center">
  ![Imagen](./imgs/expansion/imagen (7).png){ width="85%" }
  <figcaption>Imagen</figcaption>
</figure>

Dependiendo del factor de forma, debemos utilizar un

**bracket**

de

**perfil alto**

o de

**pefil bajo**

## 3. Tarjetas gráficas

La tarjeta gráfica , también conocida como tarjeta de vídeo , tarjeta aceleradora de gráficos o adaptador de pantalla , es una de las más importantes del equipo, al ser la responsable de mostrar texto, imágenes y gráficos en el monitor .

Muchas placas base actuales integran esta función; sin embargo, la mayoría de los ordenadores utilizan tarjetas gráficas para potenciar y mejorar la salida de datos hacia el monitor.

Controla la apariencia, el movimiento, el color, el brillo y la claridad de las imágenes mostradas en el monitor o la televisión, procesando cada bit de datos enviado.

La mayoría de las tarjetas gráficas actuales están diseñadas para la ranura PCI Express x16; las tarjetas PCI y AGP están prácticamente extintas.

<figure markdown="span" align="center">
  ![Imagen](./imgs/expansion/imagen(1).png){ width="85%" }
  <figcaption>Imagen</figcaption>
</figure>

### 3.1. Componentes

### Componentes

#### GPU (Graphics Processing Unit)

**Procesador**

dedicado

**específicamente al procesamiento de gráficos**

para disminuir la carga de la CPU. Está

**optimizado para el cálculo en coma flotante**

, predominante en las funciones 3D. Busca mayor realismo en los efectos.

Implementa determinadas

**operaciones**

gráficas llamadas

**primitivas**

que están optimizadas para el procesamiento gráfico como la primitiva

**antialiasing**

(suaviza los bordes de las figuras).

**Frecuencia de reloj del núcleo**

o núcleo gráfico (core) actualmente lo normal es entre 400 MHz y 900 MHz.

Dos grandes fabricantes:

**nVIDIA**

y

**ATI**

(comprada por

**AMD**

),
 pero las empresas que fabrican tarjetas gráficas como ASUS, MSI o 
GIGABYTE optan por utilizar estos componentes y ya tienen en el mercado 
tarjetas gráficas que van equipadas con dos GPU, como puede ser la ATI 
ASUS 3870 X2.

#### Memoria de vídeo

En el caso de que la tarjeta gráfica esté integrada en

[la placa base](https://aules.edu.gva.es/fp/mod/book/view.php?id=453117)

, se utilizará la memoria RAM propia del ordenador, y si se instala

**como tarjeta de expansión**

, la tarjeta gráfica dispondrá de una

**memoria propia**

. Dicha memoria es la memoria de vídeo o VRAM.

Asi, pues existen memorias gráficas de dos tipos:

- **Dedicada**

  : cuando la tarjeta gráfica o la

  **GPU dispone**

  exclusivamente para sí esas memorias, esta manera es la más eficiente y la que mejores resultados da.

- **Compartida**

  : cuando se utiliza memoria en detrimento de la memoria de acceso aleatorio (RAM).

<figure markdown="span" align="center">
  ![Imagen](./imgs/expansion/imagen(2).png){ width="85%" }
  <figcaption>Imagen</figcaption>
</figure>

Su tamaño oscila entre los 128 MB y 1 TB.

La memoria actual está

**basada en tecnología DDR**

, destacando GDDR2, GDDR3, GDDR4, GDDR5 y GDDR6, y en la nueva tecnología de AMD HBM (High Bandwidth Memory) y HBM2.

La

**frecuencia de reloj**

de la memoria se encuentra en la mayoría de las tarjetas actuales entre
 400 MHz y 14 GHz. Frecuencias de reloj de memoria por tecnología:

La memoria de vídeo tiene los siguientes

**parámetros**

:

- **Altura**

  : número de píxeles desde la parte inferior a la parte superior de la pantalla.

- **Anchura**

  : número de píxeles desde la parte izquierda a la parte derecha de la pantalla.

- **Profundidad del color**

  : número de bits usados para cada píxel o cantidad de colores que puede
 mostrar una imagen. Cuantos más colores mejor calidad y por tanto, 
mayor fidelidad con el original.

- **Resolución**

  : 
número de puntos (píxeles) que es capaz de presentar una tarjeta de 
vídeo en la pantalla, tanto en horizontal como en vertical. Por ejemplo,
 800 x 600 significa que la imagen está formada en total por 600 líneas 
horizontales de 800 puntos cada una.

La resolución se expresa como ancho x alto.

- **Cantidad de memoria de una tarjeta gráfica**

  (en bytes) : ancho x alto x profundidad de color / 8.

**A mayor cantidad de memoria de vídeo**

,
 mayor será la cantidad de texturas que la tarjeta gráfica podrá 
controlar cuando muestre gráficos 3D. Las tarjetas gráficas deben tener 
memoria suficiente para almacenar la información de los datos de una 
pantalla.

La capacidad de la memoria también es importante porque afecta el número y la resolución de imágenes que puede almacenarse.

<figure markdown="span" align="center">
  ![Imagen](./imgs/expansion/imagen (9).png){ width="85%" }
  <figcaption>Imagen</figcaption>
</figure>

<figure markdown="span" align="center">
  ![Imagen](./imgs/expansion/imagen (10).png){ width="85%" }
  <figcaption>Imagen</figcaption>
</figure>

##### ¿Cómo calcular la memoria necesaria que se necesita para cierta configuración de pantalla?

- 1280 x 1024 con 32 bits por píxel

- 1280 x 1024 = 1.310.720 píxeles:

- Cada uno de esos píxeles necesita 32 bits para almacenar su color.: 1.310.720 x 32 = 41.943.040 bits

- Tranformando a Bytes:  41.943.040 bits / 8 = 5.242.880 Bytes

- 5.242.880 / 1024 = 5.120 KBytes / 1024 = 5 MB

##### ¿Cómo calcular la memoria necesaria que se necesita para cierta configuración de pantalla?

- 1920 x 1200 con 32 bits por píxel

- 1920 x 1200 = 2.304.000 píxeles

- Cada uno de esos píxeles necesita 32 bits para almacenar su color: 2.304.000 x 32 = 73.728.000 bits

- Tranformando a Bytes:  73.728.000 bits / 8 = 9.216.000 Bytes

- 9.216.000 / 1024 = 9.000 KBytes / 1024 = 8.79 MB =  ~ 9MB

Recuerda las resolluciones de pantalla estandar:

<figure markdown="span" align="center">
  ![Imagen](./imgs/expansion/imagen (11).png){ width="85%" }
  <figcaption>Imagen</figcaption>
</figure>

#### RAMDAC

El

**convertidor digital-analógico de memoria de acceso aleatorio**

(RAMDAC) es un conversor de señal digital a señal analógica de memoria RAM. Se usa en la

**transformación de señales digitales**

(con las que trabaja la tarjeta gráfica)

**a señales analógicas**

(para poder ser interpretadas por algunos monitores).

El
 RAMDAC es capaz de dar soporte a diferentes velocidades de refresco del
 monitor (se recomienda trabajar a partir de 75 Hz, nunca con menos de 
60).

Debido a la popularidad de los monitores digitales y a que parte de su funcionalidad se ha trasladado a

[la placa base](https://aules.edu.gva.es/fp/mod/book/view.php?id=453117)

,

*el RAMDAC está quedando obsoleto.*

La
 frecuencia de actualización (o velocidad de refresco) es el número de 
veces que se dibuja la imagen en la pantalla por segundo y se mide en 
herzios. Por ejemplo, 72 Hz significa que la pantalla se dibuja 72 veces
 por segundo.

### 3.2. GPU y Arquitectura

Los procesadores gráficos tienen una infinidad de parámetros de rendimiento y además están construidos bajo distintas arquitecturas y fabricantes. En esta lista solamente podremos las últimas tecnologías de cada fabricante, así como las características que debes ser tenidas en cuenta para cada uno de ellos.

##### Arquitectura Turing (Nvidia)

Toda tarjeta gráfica que lleve en su nombre RTX, será de tecnología Turing, y es la tecnología más novedosa de la marca y que nos ofrece las tarjetas gráficas de mayor rendimiento en la actualidad. La arquitectura Turing fabrica procesadores con transistores de 12 nm y optimizados para el Ray Tracing , o trazado de rayos en tiempo real, Realidad Virtual (VR) e Inteligencia Artificial. En las características de los procesadores de las Nvidia RTX podremos identificar los núcleos CUDA , núcleos Tensor y núcleos RT (procesador de Rayos dedicados) dedicados), y la frecuencia de reloj del procesador. Mientras mayores sean las cifras de estos núcleos y frecuencia, mayor rendimiento ofrecerá la tarjeta gráfica. Los núcleos CUDA ( Compute Unified Device Architecture ), también llamado CUDA Core o CUDA Cores , es como un mini procesador que se encarga de cierto tipo de instrucciones, que suelen poder ejecutarse de manera paralela con kits de desarrollo de software de NVIDIA CUDA 10, FleX y PhysX para crear simulaciones complejas, como dinámicas de partículas o fluidos para visualizaciones científicas, entornos virtuales y efectos especiales.

### Diferencias entre CPU y GPU

La

**GPU**

está especializada en cómputo intensivo,

**computación**

altamente

**paralela**

y sus transistores se dedican al procesamiento de datos en lugar de almacenamiento en cache de datos y control de flujo

La

**CPU**

**pocos**

**núcleos**

pero

**complejos**

.

La

**GPU**

tiene

**miles**

de

**núcleos**

**sencillos**

, orientados al cálculo (unidades de cálculo FPU independientes).

La GPU no sigue la arquitectura Von Neuman, si no el Modelo Circulante basado en la Segmentación y el Procesamiento Paralelo.

La CPU sigue la arquitectura Von Neuman.

<figure markdown="span" align="center">
  ![Imagen](./imgs/expansion/imagen(3).png){ width="85%" }
  <figcaption>Imagen</figcaption>
</figure>

### 3.3. Interfaces con placa base

Existen varios tipos de interfaces que se utilizan para conectar las tarjetas gráficas, aunque en la actualidad prácticamente han desaparecido los formatos PCI y AGP y solo se usa el PCI Express x16. Actualmente se están vendiendo tarjetas gráficas que además de los 16 lanes (x16) soportan el estándar 2.1, lo que supone una tasa de transmisión de 1 GB/s por lan, llegando a los 16 GB/s de ancho de banda (1 GB/s x 16).

<figure markdown="span" align="center">
  ![Imagen](./imgs/expansion/imagen (12).png){ width="85%" }
  <figcaption>Imagen</figcaption>
</figure>

<figure markdown="span" align="center">
  ![Imagen](./imgs/expansion/imagen (13).png){ width="85%" }
  <figcaption>Imagen</figcaption>
</figure>

<figure markdown="span" align="center">
  ![Imagen](./imgs/expansion/imagen (14).png){ width="85%" }
  <figcaption>Imagen</figcaption>
</figure>

### 3.4. Salidas/conectores de la tarjeta gráfica

### SVGA (Super Video Graphic Array - Super VGA)

Conjunto de estándares gráficos diseñados en la década de 1990 para dispositivos CRT; monitor analógico de rayos catódicos.

Sufre de ruido eléctrico y distorsión por la conversión de digital a analógico. El conector utilizado es el D-sub de 15 pines (DB-15).

<figure markdown="span" align="center">
  ![Imagen](./imgs/expansion/imagen (16).png){ width="85%" }
  <figcaption>Imagen</figcaption>
</figure>

### DVI

Sustituto del anterior, fue diseñado para obtener la máxima calidad de visualización en las pantallas digitales. El DVI también tiene implementado un sistema de mayor envergadura denominado DVI Dual-Link, que permite resoluciones de 2048 × 1536 píxeles.

Hace corresponder directamente un píxel a representar con uno del monitor en su resolución nativa. Interfaz de video diseñada para obtener la máxima calidad de visualización en pantallas digitales (TFT, LCD, Plasma). La ventaja frente a VGA está en que el monitor (que es digital) ya recibe la información en formato digital y no se deben hacer conversiones.

<figure markdown="span" align="center">
  ![Imagen](./imgs/expansion/imagen (17).png){ width="85%" }
  <figcaption>Imagen</figcaption>
</figure>

Los conectores DVI se clasifican en tres tipos en función de qué señales admiten:

- DVI-D (solamente digital)

- DVI-A (solamente analógica)

- DVI-I (digital y analógica)

A veces se denomina DVI-DL a los conectores que admiten dos enlaces.

<figure markdown="span" align="center">
  ![Imagen](./imgs/expansion/DVI_Connector_Types.svg.png){ width="85%" }
  <figcaption>Imagen</figcaption>
</figure>

<figure markdown="span" align="center">
  ![Imagen](./imgs/expansion/M1-DA.svg.png){ width="85%" }
  <figcaption>Imagen</figcaption>
</figure>

### HDMI (High-Definition Multimedia Interface)

Se trata de una interfaz capaz de transmitir señal de vídeo estándar, mejorado o de alta definición, así como audio de alta definición (de hasta ocho canales). Actualmente se está utilizando la versión 2.1. Las especificaciones de este tipo de conector permiten un ancho de banda de 48GB/s para dar soporte de 64Hz para monitores 8K y 120Hz para 4K. Compatible con HD-DVD y Blu-Ray.

El conector estándar de HDMI tipo A (que es el que se utiliza actualmente) tiene 19 pines.

Se ha definido también una versión de 29 pines (tipo B), que permite llevar un canal de vídeo expandido para pantallas de alta resolución, superiores a las del formato 1080p.

El HDMI tipo A es compatible con un conector tipo DVI; es decir, que una tarjeta gráfica DVI puede conectarse a un monitor HDMI, y viceversa, mediante un adaptador.

<figure markdown="span" align="center">
  ![Imagen](./imgs/expansion/imagen (22).png){ width="85%" }
  <figcaption>Imagen</figcaption>
</figure>

### DisplayPort

Puerto para tarjetas gráficas creado por VESA y rival del HDMI, transfiere vídeo a alta resolución y audio.

Sus ventajas son que está libre de patentes, y por ende de regalías para incorporarlo a los aparatos, también dispone de unas pestañas para anclar el conector impidiendo que se desconecte el cable accidentalmente.

<figure markdown="span" align="center">
  ![Imagen](./imgs/expansion/imagen (23).png){ width="85%" }
  <figcaption>Imagen</figcaption>
</figure>

Cada vez más tarjetas gráficas van adoptando este sistema, aunque sigue siendo su uso minoritario, existe una versión reducida de dicho conector llamada Mini DisplayPort, muy usada para tarjetas gráficas con multitud de salidas simultáneas, como pueden ser 5.

<figure markdown="span" align="center">
  ![Imagen](./imgs/expansion/imagen (24).png){ width="85%" }
  <figcaption>Imagen</figcaption>
</figure>

Al igual que ocurre con HDMI, DisplayPort también es capaz de enviar audio, donde cada versión de dicha interfaz agrega mejoras en este apartado por norma general. Así, es capaz de transmitir audio Dolby, MAT, DRA o DTS HD con un máximo de 8 canales sin compresión a 192 kHz, 24 bits y 6,144 Mb/s.

Lo que más define a DisplayPort es la velocidad y los tipos de conectores que ha ido adquiriendo a modo de compatibilidad con el paso de las versiones.

<figure markdown="span" align="center">
  ![HDMI o DisplayPort ¿Cuál es más adecuado según el tipo de uso? - MuyComputer](./imgs/expansion/2Q==){ width="85%" }
  <figcaption>HDMI o DisplayPort ¿Cuál es más adecuado según el tipo de uso? - MuyComputer</figcaption>
</figure>

<figure markdown="span" align="center">
  ![Imagen](./imgs/expansion/imagen (25).png){ width="85%" }
  <figcaption>Imagen</figcaption>
</figure>

Actualmente, VESA ha presentado la versión 2.0, la cual es la más avanzada hasta la fecha y trae grandes mejoras. DisplayPort comenzó con una velocidad máxima de 8,64 Gb/s en mayor de 2006, apoyándose en un cableado de cobre y fibra, con soporte para HDCP y DPCP y sonido 7.1 digital.

Con el paso de las versiones se han añadido soporte para MST, mejoras de la sincronización de audio y vídeo, adaptadores pasivos, soporte para 4K, 8K y 16K (15360 x 8460 @ 60 Hz), soporte para HDMI 2.0, DockPort, un aumento de velocidad de hasta 77,4 Gb/s, mapeo del flujo de datos, soporte para Thunderbolt y USB-C y un menor consumo.

Actualmente, más de 280 fabricantes apoyan directamente esta interfaz, en especial Intel, AMD y NVIDIA, los cuales están apostando muy fuerte por ella debido a sus mayores posibilidades y velocidades frente a HDMI.

### Thunderbolt

La interfaz

**Thunderbolt**

es un estándar para la

**transmisión de datos y energía**

en diferentes tipos de dispositivo. Originalmente conocido como Light Peak, fue desarrollado por Intel en colaboración con Apple, que fue la única que dio respaldo comercial realmente sólido a esta interfaz, a la que dio ese nombre por el que fue conocida a posteriori. Su tercera versión fue presentada en 2015, y es la que nos ocupa hoy.

Existe un poco de confusión a la hora de hablar de esta tecnología, sobre todo a la hora de diferenciarla del USB de tipo C. Esto es así porque el

**Thunderbolt 3 utiliza un puerto USB-C**

, o sea que su aspecto es el mismo exteriormente, pero

**no todos los USB de tipo C son Thunderbolt**

debido a diferencias en su interior.

<figure markdown="span" align="center">
  ![Imagen](./imgs/expansion/imagen (26).png){ width="85%" }
  <figcaption>Imagen</figcaption>
</figure>

La

**velocidad de transmisión**

del Thunderbolt 3 es de hasta

**40 Gbps (5 GB/s)**

, cuatro veces más que el USB 3.1 y el Thunderbolt original. que ofrecían 10 Gbps. (los discos duros SSD andan entre 200 y 550 MB/s). Además, también soporta conexiones DisplayPort 1.2, HDMI 2.0, y Ethernet 10 Gigabit.

Gracias a la velocidad, el Thunderbolt 3 puede utilizarse para conectar monitores de alta resolución al mismo tiempo. Por ejemplo, uno 5K, dos 4K, o tres FullHD. También permite enchufar las siempre exigentes tarjetas gráficas externas, todo con un mismo conector que también servirá para estar cargando tu equipo.

### Tarjetas gráficas mediante USB

Aunque existen en el mercado desde hace tiempo, no han tenido mucha aceptación entre el público debido

a su poca potencia.

Son relativamente baratas y normalmente se van a utilizar para dotar a un equipo de más monitores o proyectores en paralelo.

La mayoría dispone de los tipos de salida VGA y DVI, aunque aprovechando la tecnología USB 3.0 se están fabricando tarjetas gráficas USB con salida HDMI.

<figure markdown="span" align="center">
  ![Imagen](./imgs/expansion/imagen (27).png){ width="85%" }
  <figcaption>Imagen</figcaption>
</figure>

<figure markdown="span" align="center">
  ![Imagen](./imgs/expansion/imagen (28).png){ width="85%" }
  <figcaption>Imagen</figcaption>
</figure>

### Diferencias:

<figure markdown="span" align="center">
  ![Imagen](./imgs/expansion/imagen (29).png){ width="85%" }
  <figcaption>Imagen</figcaption>
</figure>

### Adaptadores

Dada la diversidad de conectores que hemos visto, existen una serie de apatados entre uno y otros:

##### Desde VGA a DVI

<figure markdown="span" align="center">
  ![Imagen](./imgs/expansion/imagen (30).png){ width="85%" }
  <figcaption>Imagen</figcaption>
</figure>

##### De VGA a HDMI

<figure markdown="span" align="center">
  ![Imagen](./imgs/expansion/imagen (31).png){ width="85%" }
  <figcaption>Imagen</figcaption>
</figure>

##### De DisplayPort a DVI

<figure markdown="span" align="center">
  ![Imagen](./imgs/expansion/imagen (32).png){ width="85%" }
  <figcaption>Imagen</figcaption>
</figure>

De DisplayPort a HDMI

<figure markdown="span" align="center">
  ![Imagen](./imgs/expansion/imagen (33).png){ width="85%" }
  <figcaption>Imagen</figcaption>
</figure>

### 3.5. Tarjetas gráficas integradas y dedicadas

Las unidades de procesamiento gráfico se clasifican normalmente en dos tipos: GPU integradas y GPU dedicadas. Las tarjetas gráficas integradas tienen la ventaja de ser más baratas , lo que a su vez conduce a un ordenador menos costoso. También disipan mucho menos calor que las GPU dedicadas y, por lo tanto, permiten máquinas compactas con sistemas de refrigeración relativamente pequeños. Además, un portátil que se basa únicamente en gráficas integradas será más eficiente en el consumo de energía para una mayor duración de la batería. La compensación es, por supuesto, el rendimiento que obtienes. Las GPU integradas son perfectas para tareas casuales como ver vídeos y procesar documentos gráficos. Las unidades dedicadas o discretas , por otra parte, vienen con su propia memoria de vídeo , que es usada de manera exclusiva para el procesamiento gráfico. Además cuestan más y requieren fuentes de alimentación y sistemas de refrigeración elaborados. Para juegos intensos, son la mejor opción.

La recomencación de uso sería:

- **Procesador con tarjeta gráfica integrada**

  : Usuarios que son jugadores ocasionales que no le importa bajar la resolución (720p) y sus filtros (calidad baja o media), tareas básicas: ofimática, navegación web, ver vídeos o retocar a nivel amateur retoque fotográfico.

- **Tarjeta gráfica dedicada**

  : Usuarios que quieren jugar fluidamente, con buena resolución y gráficamente al máximo en su ordenador. También da un empujón en el renderizado de vídeos o en aplicaciones que sacan el máximo provecho a su tarjeta gráfica. Sin olvidarnos, de aquellos usuarios que quieren estar siempre a la última.

### Diferentes tipos de tarjetas integradas

#### iGPU

Algunas CPU pueden incorporar un procesador gráfico llamado

**iGPU**

, que no es sino una GPU integrada pero que funciona de manera independiente. De esta manera, se consigue que sin necesidad de una tarjeta gráfica dedicada podamos visualizar el contenido en un monitor, aunque en estos casos el rendimiento es bastante bajo debido a las limitaciones físicas que tienen.

<figure markdown="span" align="center">
  ![Imagen](./imgs/expansion/imagen(5).png){ width="85%" }
  <figcaption>Imagen</figcaption>
</figure>

Como características principales tenemos:

- Comparte encapsulado normalmente con la CPU pero también podemos encontrar versiones soldadas a la placa.

- Una iGPU consume RAM del equipo.

- Las iGPU integradas tienen una pequeña cantidad de memoria que puede ser de diferentes tipos pero a la hora de cargar juegos o aplicaciones gráficas intensivas recurren a la RAM principal y la utilizan como memoria de vídeo.

- La RAM del PC se verá reducida en relación al consumo de la iGPU. Si nuestro equipo tiene 4 GB y la iGPU consume 2 GB sólo tendremos otros 2 GB para el sistema.

- Al recurrir a la RAM principal en el ancho de banda de la iGPU influye la velocidad de trabajo de la memoria (Hay que apostar por configuraciones en doble canal o superiores para mejorar el rendimiento).

#### APU

Como una variante de las CPU con iGPU, en 2011 AMD lanzó el concepto de

**APU**

, que se diferencia de éstas en que el hardware para gráficos que integra no solo es bastante más potente (de hecho, AMD las vende como dispositivos para jugar), sino que tienen una diferencia fundamental, la arquitectura HSA (heterogénea).

<figure markdown="span" align="center">
  ![Imagen](./imgs/expansion/imagen (34).png){ width="85%" }
  <figcaption>Imagen</figcaption>
</figure>

La arquitectura HSA permite el procesamiento paralelo y permite que la GPU trabaje junto con la CPU , lo que da un rendimiento general superior.

De este modo, la APU elimina el bus entre la CPU y la GPU para integrar ambas unidades en el mismo chip. Por tanto, una APU es más rápida en tareas gráficas pequeñas , que una CPU y GPU por separado.

Obviamente, tiene sus limitaciones : no podemos pretender que los gráficos integrados de la APU den el mismo rendimiento que una GPU dedicada en, por ejemplo, videojuegos. Sin embargo, en tareas pequeñas, tener una GPU puede ser un malgasto, siendo mejor opción una APU.

##### 

##### 

##### Versiones:

**AMD: APU:**

- Excavator architecture (2016): Bristol Ridge and Stoney Ridge

- Zen architecture (2017): Raven Ridge INTEL HD and Iris Graphics

**IntelHD and Iris Graphics**

- Iris Pro Graphics 6200 (128MB memoria dedicada de vídeo).

- Intel HD Graphics 6000 (64MB de memoria dedicada de vídeo).

### 3.6. SLI/Crossfire

El procesamiento en paralelo es un método para conectar dos o más tarjetas de video PCI Express para producir una sola señal de salida que incremente la capacidad de procesamiento disponible para gráficos En un principio las dos tarjetas deberían ser idénticas mismo fabricante y modelo, sin embargo, hoy no es necesario siempre que se empleen las últimas versiones de los controladores suministrados por el fabricante El excedente de memoria no se utilizaría en el funcionamiento conjunto y además las GPU de las tarjetas deben de ser idénticas . Según sea el fabricante de GPU se la denomina

- **SLI**

  (Scalable Link Interface), de la empresa

  **nVidia**

- **Crossfire**

  de la empresa

  **ATI/AMD**

<figure markdown="span" align="center">
  ![GeForce GTX 980 TI SLI](./imgs/expansion/imagen (37).png){ width="85%" }
  <figcaption>GeForce GTX 980 TI SLI</figcaption>
</figure>

<figure markdown="span" align="center">
  ![Imagen](./imgs/expansion/imagen (38).png){ width="85%" }
  <figcaption>Imagen</figcaption>
</figure>

Para unir dos o más tarjetas gráficas se emplea un conector que hace de puente entre ellas, normalmente en la parte superior, y solamente una de las tarjetas se conectara con el monitor.

En todo caso, es una tecnología que no esta prestando los servicios que se esperaban . El muti-GPU parece que solo aprovecha juegos 4K y ofrecen problemas para comportase como se espera, por lo que la evución de estas tecnologías dejo de promoverse en 2018

### 3.7. Refrigeracíon

Las tarjetas gráficas alcanzan temperaturas muy altas debido a carga trabajo si no se soluciona puede fallar o averiarse. Solución dispositivos refrigerantes tipos:

##### Disipador dispositivo pasivo:

- Sin partes móviles y por tanto silencioso.

- Hecho de material conductor del calor que lo extrae de la tarjeta.

- Suelen ser bastante voluminosos.

<figure markdown="span" align="center">
  ![Imagen](./imgs/expansion/imagen (39).png){ width="85%" }
  <figcaption>Imagen</figcaption>
</figure>

##### Ventilador dispositivo activo:

- Con partes móviles y produce ruido.

- Aleja el calor emanado de la tarjeta al mover el aire cercano.

- Es más eficiente que un disipador

Ambos tipos de dispositivos refrigerantes son compatibles entre sí y suelen montarse juntos en las tarjetas gráficas: un disipador sobre la GPU (componente que más calor genera) extrae el calor y un ventilador sobre él aleja el aire caliente del conjunto. Además de los dispositivos refrigerantes propios de la tarjeta, se pueden instalar en el ordenador otros ventiladores externos.

### 3.8. Alimentación

Actualmente casi todas las tarjeta gráficas dedicadas requieren alimentación auxiliar , dado que estas tarjetas de expansión, cada vez consumen más y el puerto PCIe de nuestra placa base no es capaz de suministrar más de 75 W de potencia, es habitual que incluso modelos de gama baja necesiten este tipo de alimentación.

En un principio esta alimentación adicional no era necesaria, pero poco a poco la potenia de las tarjetas ha demandado más energía y ha propicidado la necesidad de suministro externo.

A continuación tenemos los diferentes contectores usado a lo largo de los años para alimentar las tarjetas gráficas:

<figure markdown="span" align="center">
  ![Imagen](./imgs/expansion/imagen (41).png){ width="85%" }
  <figcaption>Imagen</figcaption>
</figure>

Inicialmente se utilizaban conectores Molex, pero en la actualidad es más habitual encontrar conectores PCI-E de 6 u 8 pines.

<figure markdown="span" align="center">
  ![Imagen](./imgs/expansion/imagen (42).png){ width="85%" }
  <figcaption>Imagen</figcaption>
</figure>

Es necesario comprobar que la potencia de la fuente de alimentación del equipo sea suficiente. Las nuevas tarjetas gráficas de gran potencia necesitan una alimentación específica que dependerá del modelo y sus prestaciones.

<figure markdown="span" align="center">
  ![Imagen](./imgs/expansion/imagen (43).png){ width="85%" }
  <figcaption>Imagen</figcaption>
</figure>

El cable de alimentación auxiliar para tarjetas gráficas se caracteriza por tomar toda su potencia desde el raíl +12 V de la fuente de alimentación. Ello es así porque las gráficas solo usan ese tipo de alimentación para funcionar. Los colores de los cables individuales suelen ser amarillo (para la tensión) y negro para el neutro. También hay cables adaptadores que permiten usar conectores de alimentación molex o SATA para suplir la ausencia de estos en nuestra fuente de alimentación. Este tipo de cable es más moderno. Inicialmente se usaban adaptadores que se conectaban a dos conectores molex de la fuente de alimentación. De hecho, hoy en día, este tipo de adaptador de alimentación sigue siendo el más extendido. Y el que más suelen distribuir los fabricantes de tarjetas gráficas con sus modelos. Como ya se ha comentado, el conector de alimentación es del tipo 6+2. Esto significa que su cuerpo principal es un conector de 6 pines. Al que se le pueden añadir dos pines extra, si la gráfica lo necesitara. Esto da mucha flexibilidad a los fabricantes de gráficas y fuentes. Así como beneficia a los usuarios, en el caso de tener alguna de las primeras gráficas que usaban solo el conector inicial de 6 pines. El motivo de la existencia de los dos tipos de conectores, es que uno de ellos es capaz de proporcionar 75 W extra (el de 6 pines), mientras que el otro conector proporciona hasta 150 W de potencia extra (el de 8 pines). A esto hay que sumarle los 75 W que proporciona la ranura PCIe de la placa base a la tarjeta gráfica.

Fuente: Tipos de alimentación para tarjetas gráficas

### 3.9. Multimonitor

Con la bajada de precios de los monitores actuales y el aumento de la potencia de las tarjetas gráficas, cada vez se está extendiendo más la utilización de varios monitores en paralelo, tanto para juegos como para trabajo (diseño gráfico, hojas de cálculo muy grandes, etc.). Para ello y dependiendo del hardware del que dispongamos, se puede llegar a utilizar más de seis pantallas simultáneamente con un único ordenador. Dispondremos de varios formatos de trabajo, entre ellos:

- **En espejo**

  : Se replica la imagen en todos los monitores. En todos se ve lo mismo.

- **Escritorio extendido**

  : Se detectan y enumeran los monitores, y en cada uno de ellos se muestra parte de nuestro escritorio. Puede orientarse en vertical u horizontal.

<figure markdown="span" align="center">
  ![Imagen](./imgs/expansion/imagen(6).png){ width="85%" }
  <figcaption>Imagen</figcaption>
</figure>

Para realizar estas tareas de configuración utilizaremos normalmente el sistema operativo o el software propietario de la marca de nuestra tarjeta gráfica:

<figure markdown="span" align="center">
  ![Imagen](./imgs/expansion/imagen (50).png){ width="85%" }
  <figcaption>Imagen</figcaption>
</figure>

## 4. Tarjetas de red

También conocidas como adaptador de red o NIC ( Network Interface Card ) y se usan para conectar ordenadores entre sí para compartir recursos y poder formar una red. Hay distintos tipos de tarjetas de red, en función del tipo de cable o arquitectura que se utilice en la red (coaxial fino, coaxial grueso, fibra de vidrio, etc.) pero el más utilizado es del tipo Ethernet con un conector RJ-45 (la mayoría de placas base la tienen integrada).

Por otra parte, cada vez está más extendido el uso de redes Wi-Fi .

<figure markdown="span" align="center">
  ![Imagen](./imgs/expansion/imagen(7).png){ width="85%" }
  <figcaption>Imagen</figcaption>
</figure>

### 4.1. Tarjeta para redes cableadas

Las redes pequeñas se denominan redes de área local o LAN (Local Area Network). En este caso, la red se establece con un cable y componentes hardware que comunican todos los ordenadores. La tarjeta de red comunica al ordenador con una red local, y suele instalarse en una ranura PCIe de la placa, aunque también tenemos otras alternativas tal y como veremos a continuación.

Comencemos viendo un ejemplo de tarjeta de red con interfaz PCIe 1x , que viene acompañada de sus dos brackets para ajustarar a cajas con perfil alto o bajo.

### Conectores

La salida de conexión de la tarjeta de red debe ser del mismo tipo que el cableado a usar conector más utilizado RJ-45 para el cable de par trenzado.

Tipos de cable de par trenzado:

Antes se utilizaban los conectores BNC para el tipo de cable coaxial pero su uso está obsoleto. Existen tarjetas de red híbridas que permiten los dos sistemas de conexión.

Cable BNC:

Disponen de LEDs que se iluminan según la actividad de la tarjeta

### 

### Dirección MAC (Media Control Address)

Se trata de un código identificador de 48 bits (6 bytes) individual que corresponde de forma única a una tarjeta. Cada dispositivo tiene su propia MAC determinada y configurada por el IEEE (los últimos 24 bits) y el fabricante (los primeros 24 bits). Se codifican en hexadecimal: son 12 números en hexadecimal agrupados de 2 en 2. Por ejemplo: 00-16-E6-5E-7B-74 . Las direcciones MAC o direcciones físicas son únicas a nivel mundial son escritas en el hardware en el momento de su fabricación de forma binaria.

### Velocidad

Una tarjeta de red puede trabajar a distintas velocidades, en función de la tecnología y los estándares que soporte. Estándares más utilizados:

- **Ethernet**

  10 Mb/s.

- **Fast Ethernet**

  100 Mb/s.

- **Gigabit Ethernet**

  1000 Mb/s.

Es común que las tarjetas de red actuales soporten las 3 velocidades y se adapten a la velocidad del resto de los componentes de la red.

##### Wake on LAN (WoL)

Estándar de redes de computadoras Ethernet que permite encender remotamente ordenadores apagados mediante el envío de un Magic Packet, paquete especial que recibe la tarjeta de red. El soporte WoL está implementado en la placa base del ordenador y la mayoría de las placas base modernas cuentan con un controlador. Ethernet que incorpora WoL sin necesidad de un cable externo. Las placas base antiguas necesitaban un conector WAKEUP-LINK que debía estar enchufado a la tarjeta a través de un cable de 3 pines especial. Debe estar habilitado en la sección administración de energía de la BIOS. También es posible que sea necesario configurar el equipo para proveer energía a la tarjeta de red cuando el sistema está apagado. Puede ser necesario activar la características WoL en la tarjeta de red (cómo hacerlo dependerá del sistema operativo y de los drivers). En tarjetas con soporte WoL que necesiten cable para recibir alimentación: debe tener un conector de 3 pines y desde ese conector debemos conectar un cable a la placa base. Tanto la tarjeta de red, como la placa base han de soportar esta tecnología.

### Tarjeta de red mediante adaptador USB

Este dispositivo consiste en un adaptador de red con un puerto USB y un puerto RJ-45 10/100/1000 Mb/s Fast/Giga Ethernet. Se puede conectar a cualquier ordenador o portátil dotado de un puerto USB, convirtiendo así la interfaz USB en un puerto de red LAN tipo Ethernet o Fast/Giga Ethernet 10/100/1000 Mb/s. Como la mayoría de dispositivos USB, se elimina la necesidad de instalar y utilizar tarjetas PCI para ofrecer conectividad LAN al ordenador.

### 4.2. Tarjeta para redes Wifi

Wi-Fi es una marca de la Wi-Fi Alliance, la organización comercial que adopta, prueba y certifica los estándares 802.11 .

Es un sistema de envío de datos para redes informáticas que usa ondas de radio en lugar de cables:

- Instalación rápida.

- Menos seguridad que con cable.

- Menor velocidad de transmisión de datos que con cable.

Transmite la información mediante tarjetas de red con una o varias antenas a través de routers o puntos de acceso. Los datos pueden ser enviados mediante algoritmos y procesos de cifrado para mejorar la seguridad. En el mercado se pueden encontrar tarjetas de expansión de red para Wi-Fi en formato PCIe pero se está imponiendo el uso de adaptadores red Wi-Fi en formato stickers USB por su facilidad de instalación y portabilidad.

Las tarjetas de expansión de red Wi-Fi habilitan al equipo para acceder a este tipo de redes y también tienen dirección MAC.

## Clases de normas IEEE 802.11 para WLAN

Lo de WMAN y WWLAN está muy bien, pero consideramos que no es un tema a tratar aquí, ya que estamos centrándonos en las redes inalámbricas ámbito local .

Entonces será importante conocer las distintas versiones del estándar o nombra IEEE 802.11 para así conocer las velocidades y características que aporta cada versión.

#### IEEE 802.11a/b/g

Estos estándares se consideran identificadores de canales y frecuencias por donde se conectarán los hosts a la WLAN.

Con 802.11a opera sobre las bandas de 5 GHz a 20 MHz y 2,4 GHz , las dos más utilizadas en Wi-Fi al menos en la zona de Europa. Además, en esta zona opera junto a 802.11h que realiza ciertas modificaciones en el control dinámico de frecuencias y potencias de transmisión para que no existan interferencias con señales por satélite y sistemas de radar.

802.11 b y g están operando solamente en la banda de 2,4 GHz dotándola de 11 canales para WiFi de los cuales normalmente se utilizan el 1, 6 y 11. En esta banda se opera a una frecuencia de 25 MHz como ancho de banda. La velocidad de transmisión en la versión “b” es de 54 Mbps sin capacidad de envío OFDM implementado en la última versión disponible.

#### IEEE 802.11n

Esta versión del estándar empezó a operar en 2008 aunque se definió en 2004. La velocidad asciende a los 600 Mbps en conexiones como máximo de 3×3 (3 antenas). Utiliza de forma simultánea las bandas de 2,4 GHz y 5 GHz . Fue el primero en implementar la tecnología MIMO (Multiple Input – Multiple Output) que permite usar varios canales a la vez para el envío y recepción de datos con hasta 3 antenas.

<figure markdown="span" align="center">
  ![Imagen](./imgs/expansion/imagen (63).png){ width="85%" }
  <figcaption>Imagen</figcaption>
</figure>

Aún no llegamos a tasas de velocidad comparables a cableado LAN, pero el poder utilizar ambas frecuencias con un mismo punto inalámbrico toda a los dispositivos de gran cobertura.

##### IEEE 802.11ac

También se denomina WiFi 5 y fue implementado en el año 2014 y a día de hoy la mayoría de aparatos trabajan sobre esta versión. En este caso es una versión que solamente opera en la banda de 5 GHz para proporcionarnos velocidades de 433 Mbps en conexiones con una antena (1×1) y hasta 1,3 Gbps en 3×3 . Su máxima transferencia será de 3,39 Gbps utilizando 4 antenas a una frecuencia de 160 MHz o 6,77 Gbps con 8 antenas.

Este estándar implementa tecnología MU-MIMO con hasta 8 flujos de datos con ancho de bandas de hasta 160 MHz y 256 QAM . Normalmente opera junto a 802.11n para los dispositivos que utilicen la banda de 2,4 GHz.

##### IEEE 802.11ax

<figure markdown="span" align="center">
  ![Imagen](./imgs/expansion/imagen (64).png){ width="85%" }
  <figcaption>Imagen</figcaption>
</figure>

Esta es la nueva versión también denominada WiFi 6 y WiFi de 6ª generación implementada en 2019 y que muchos equipos ya tienen soporte gracias al nuevo hardware. Además de MU-MIMO, se introduce la nueva tecnología OFDMA que mejora la eficiencia espectral de la red para WLAN en donde haya conectados gran cantidad de usuarios. Por ello es un estándar que sobre todo aumenta sus prestaciones con grandes cargas de clientes y transmisiones simultaneas.

Opera sobre las frecuencias de 2,4 GHz y 5 GHz , y soporta conexiones 4×4 y 8×8 en ambos casos. La velocidad de transmisión aumenta hasta los 11 Gbps con la frecuencia de 160 MHz y 1024QAM.

<figure markdown="span" align="center">
  ![Imagen](./imgs/expansion/imagen (65).png){ width="85%" }
  <figcaption>Imagen</figcaption>
</figure>

<figure markdown="span" align="center">
  ![Imagen](./imgs/expansion/imagen (66).png){ width="85%" }
  <figcaption>Imagen</figcaption>
</figure>

### 

### Tarjetas de Red Wi-Fi USB

Actualmente están apareciendo en el mercado tarjetas de red Wi-Fi que se conectan a través de los puertos USB. Hay varios tipos en función de las necesidades del usuario:

- **Nanowireless**

  : tarjetas de tamaño muy pequeño que se colocan en el conector USB para dotar al equipo de funcionalidad Wi-Fi. Apenas sobresalen, son muy baratas y de cómodo transporte.

<figure markdown="span" align="center">
  ![Imagen](./imgs/expansion/imagen (67).png){ width="85%" }
  <figcaption>Imagen</figcaption>
</figure>

<figure markdown="span" align="center">
  ![Imagen](./imgs/expansion/imagen (68).png){ width="85%" }
  <figcaption>Imagen</figcaption>
</figure>

- **Tarjetas con antena externa**

  : tarjetas que disponen de un conector para acoplar una antena externa. Normalmente este conector es de tipo RP-SMA. El objetivo de este tipo de tarjeta+antena es el de potenciar la señal de emisión/recepción del equipo. Por ejemplo, una tarjeta de red Wi-Fi por USB como la Blueway alcanza 2W de potencia y dispone de una antena de 15 dB.

<figure markdown="span" align="center">
  ![Imagen](./imgs/expansion/imagen (69).png){ width="85%" }
  <figcaption>Imagen</figcaption>
</figure>

## 5. Tarjeta de sonido

Dispositivo que permite la reproducción , grabación y digitalización del sonido , normalmente a través de software específico. Las placas base actuales normalmente disponen del sistema de sonido integrado y suelen ser de calidad, así que es poco usual ampliar con tarjetas de expansión de sonido.

<figure markdown="span" align="center">
  ![Imagen](./imgs/expansion/imagen(9).png){ width="85%" }
  <figcaption>Imagen</figcaption>
</figure>

Normalmente la encontramos ncorporada e la placa base. Se añade una tarjeta de sonido si se necesita un uso profesional (músicos, compositores ...)

- Combinado con un software específico, permite la reproducción, grabación y digitalización del sonido

- Actualmente encontramos conexiones PCI-e 1x, PCI y USB

### 5.1. Canales y polifonia

### Multicanal

Se denomina audio multicana l o sonido multicanal al uso de múltiples pistas de audio para reconstruir el sonido en un sistema de múltiples altavoces o de sonido envolvente. No debe confundirse el sonido multicanal con altavoces de 2 vías o 3 vías (altavoces), puestos que estos últimos utilizan un solo canal de audio por altavoz aunque utilicen varios altavoces para reproducirlo según la frecuencia. Para definir las distintas configuraciones de altavoces utilizadas, se usan dos dígitos separados por un punto decimal (2.1, 3.0, 5.1, 6.1, 7.1, etc.), dependiendo de la cantidad de pistas de audio que se utilicen.

- El

  **primer dígito**

  muestra el número de canales primarios o completos, cada uno de ellos reproducido en un altavoz individual

- El

  **segundo dígito**

  se refiere a la presencia de un canal para efectos de baja frecuencia (abreviado, LFE, por sus siglas en inglés) que se reproduce en un altavoz de subgraves.

Así:

- 1.0 corresponde al sonido mono (que significa un solo canal).

- 2.0 corresponde al sonido estéreo

- 2.1 corresponde al sonido estéreo con un canal adicional para efectos de baja frecuencia.

Normalmente se denomina audio o sonido multicanal a partir de una configuración de 3 canales (2.1 o 3.0).

Las conguraciones multicanal habituales son:

<figure markdown="span" align="center">
  ![Imagen](./imgs/expansion/imagen(10).png){ width="85%" }
  <figcaption>Imagen</figcaption>
</figure>

En cuanto a la distribución sonora , los sonidos que se emiten por los distintos canales suelen ser de diferente rango para crear una sensación de sonido envolvente. Los rangos utilizados por cada canal suelen ser los siguientes:

- Los canales frontales izquierdo y derecho utilizan rango completo, emitiendo sonidos de todo tipo, a excepción de los bajos.

- El canal frontal central suele ser para rangos medios, emitiendo sonidos medios o de voz.

- Los canales laterales y traseros se utilizan para sonidos de ambientación.

- El canal de subgraves se utiliza para los sonidos graves con frecuencias de hasta 100 Hz aproximadamente.

<figure markdown="span" align="center">
  ![Imagen](./imgs/expansion/imagen (70).png){ width="85%" }
  <figcaption>Imagen</figcaption>
</figure>

En la actualidad se utilizan las tarjetas de sonido envolvente (surround), principalmente Dolby Digital 8.1 o superior.

### 5.2. Operaciones básicas

##### Operaciones Básicas

Grabación : el sonido se recoge normalmente a través de un micrófono y llega a la tarjeta a través de los conectores. Esta señal se recoge, se procesa y se almacena en el formato seleccionado. Reproducción : la señal digitalizada de un sonido se envía a la tarjeta que la procesa y la manda a través de los conectores de salida hacia los altavoces, auriculares, etc. Síntesis : procedimiento mediante el que las tarjetas reproducen sonidos a partir de datos o representaciones simbólicas, como pueden ser los códigos MIDI.

- **Síntesis FM**

  : imita el sonido de un instrumento musical manipulando la onda, su amplitud y frecuencia

- S

  **íntesis por Tabla de Onda (WaveTable)**

  : la tarjeta de sonido alberga en la memoria una colección completa de notas de instrumentos en forma de secuencias sonoras reales muy cortas previamente digitalizadas. Cuando el archivo sonoro se va reproduciendo, la tarjeta busca en la tabla y escoge el sonido que corresponde a cada caso.

- **Síntesis de Modelado Físico**

  : se simula el sonido de un instrumento musical mediante el cálculo numérico de las ondas de sonido (se tienen en cuenta parámetros como la vibración del sonido en un tubo, una cuerda, una membrana en percusión, etc).

### MIDI (Music Instrument Digital Interface)

Estándar industrial adoptado por la industria musical y el mundo informático que regula la forma en que se conectan instrumentos y ordenadores, a través de qué cables y el formato de los mensajes que se intercambian. MIDI permite a los instrumentos electrónicos musicales comunicarse bidireccionalmente con el ordenador. Los códigos MIDI no transmiten música, sino órdenes musicales. Un mensaje MIDI consta de un byte de estado seguido de un cero o más bytes de datos; cada mensaje corresponde a un evento musical del tipo de la pulsación de una tecla o un pedal, el giro o desplazamiento de un control, etc. A cada instrumento musical se le asigna asigna un código MIDI de un total de 128 disponibles.

<figure markdown="span" align="center">
  ![Imagen](./imgs/expansion/image.png){ width="85%" }
  <figcaption>Imagen</figcaption>
</figure>

### 5.3. Componentes

Los elementos que componen una tarjeta de sonido son los siguientes:

<figure markdown="span" align="center">
  ![Imagen](./imgs/expansion/imagen(11).png){ width="85%" }
  <figcaption>Imagen</figcaption>
</figure>

##### Mezclador

Se encarga de mezclar los distintos tipos de sonido que le llegan o que envía al exterior. Puede emitir sonido sintetizado y reproducido a la vez. Normalmente se controla por software.

##### ADC (Analog to Digital Converter)

Se encarga del proceso de convertir una señal de ondas analógica en su equivalente digital (denominado modulación digital). Para ello se captura el sonido almacenando en los valores de amplitud de una onda a intervalos regulares de tiempo. La amplitudde la onda de sonido determina su volumen, la frecuencia determina su escala (en el rango más grave o más aguda).

##### DAC (Digital to Analog Converter)

Realiza la demodulación digital, permitiendo reproducir el sonido tras convertir las señales digitales en analógicas.

##### DSP (Digital Signal Processor)

Pequeño microprocesador que efectúa los cálculos necesarios para gestionar el sonido, con tareas como la compresión y la descompresión de su señal. También realiza otras tareas como producir efectos de sonido, ecos, reverberaciones, coros, etc, empleando para ellos varios tipos de algoritmos.

##### Búffer

Pequeña memoria que almacena temporalmente los datos que se envían entre ordenador y tarjeta. Permite una gestión de ajustes de tiempo.

Además de los sintetizadores FM y por tablas de ondas que permiten la genearción de sonidos a partir de frecuencias y ondas.

##### Interfaz con la placa madre

Permite transmitir información entre tarjeta y ordenador. En la actualidad es a través del PCI.

### 5.4. Salidas

Las salidas de una tarjeta de sonido son las siguiente:

<figure markdown="span" align="center">
  ![Imagen](./imgs/expansion/imagen(12).png){ width="85%" }
  <figcaption>Imagen</figcaption>
</figure>

Código de colores : hay que consultar el manual pero generalmente son:

- **Rosa**

  : Entrada analógica micrófono

- **Azul**

  : Entrada analógica de línea

- **Verde**

  : Salida analógica altavoces frontales

- **Negro**

  : Salida analógica altavoces traseros

- **Plateado**

  : Salida analógica altavoces laterales

- **Naranja**

  : Salida subwoofer o S / PDIF

<figure markdown="span" align="center">
  ![Imagen](./imgs/expansion/imagen (71).png){ width="85%" }
  <figcaption>Imagen</figcaption>
</figure>

#### S/PIDF

Formato de Interfaz digital y Analógica Sony/Phillips

<figure markdown="span" align="center">
  ![Imagen](./imgs/expansion/imagen (72).png){ width="85%" }
  <figcaption>Imagen</figcaption>
</figure>

Dos posibilidades:

Analógica. Cabla Coaxial. Conectores RCA

Digital: Fibra óptica. Conector Toslink:

<figure markdown="span" align="center">
  ![Imagen](./imgs/expansion/imagen (73).png){ width="85%" }
  <figcaption>Imagen</figcaption>
</figure>

0

<figure markdown="span" align="center">
  ![Imagen](./imgs/expansion/imagen (74).png){ width="85%" }
  <figcaption>Imagen</figcaption>
</figure>

S/PDIF Digial

## 6. Tarjetas de interfaz

En este tipo se engloban todas las tarjetas que se dedican a ampliar las interfaces de nuestro sistema.

Hay tarjetas

- ATA, Bluetooth

- FireWire

- IDE

- RAID

- SCSI

- SATA

- Thunderbolt

- USB.

Es decir, añaden o complementan las que ya aporta de por sí nuestra propia placa base.

Ejemplo tarjeta puerto IDE

<figure markdown="span" align="center">
  ![Imagen](./imgs/expansion/imagen(13).png){ width="85%" }
  <figcaption>Imagen</figcaption>
</figure>

Tarjeta puertos USB

<figure markdown="span" align="center">
  ![Imagen](./imgs/expansion/imagen (75).png){ width="85%" }
  <figcaption>Imagen</figcaption>
</figure>

Tarjetas eSATA

<figure markdown="span" align="center">
  ![Imagen](./imgs/expansion/imagen (76).png){ width="85%" }
  <figcaption>Imagen</figcaption>
</figure>

Tarjetas SATA

<figure markdown="span" align="center">
  ![Imagen](./imgs/expansion/imagen (77).png){ width="85%" }
  <figcaption>Imagen</figcaption>
</figure>

Tarjeta FireWitre:

<figure markdown="span" align="center">
  ![Imagen](./imgs/expansion/imagen (78).png){ width="85%" }
  <figcaption>Imagen</figcaption>
</figure>

Por ejemplo, si queremos crear un RAID 5 pero la controladora de RAID de nuestra placa no admite ese tipo de RAID, deberemos de comprar una de estas tarjetas. De hecho, las placas base para los procesadores AMD Ryzen y Threadripper no permiten crear RAID 5 con su controladora integrada.

<figure markdown="span" align="center">
  ![Imagen](./imgs/expansion/imagen (79).png){ width="85%" }
  <figcaption>Imagen</figcaption>
</figure>

## 7. Tarjetas capturadoras de vídeo

Este tipo de tarjetas, cuando se conectan de manera interna en un PC, también se consideran tarjetas de expansión. Dado que se conectan a través de un puerto PCIe (o PCI, en el caso de las más antiguas).

Gracias a ellas, muchos de nosotros hemos podido ver la televisión directamente en nuestro ordenador. Sin embargo, para ese tipo de uso, hace tiempo que ya no se utilizan. No al menos como antiguamente.

Pero las tarjetas que se utilizan para hacer streaming y grabar partidas, son la nueva moda entre los usuarios gamers.

Existen capturadorsas te permiten grabar vídeo en 4K a 60 FPS en tu ordenador de el mismo o de otras consolas. La mayoría de capturadoras cuentan con un software que nos permite editar fácilmente lo que queremos subir posteriormente en YouTube y que tiende a ser muy sencillo de usar. En este caso no hemos podido hacer una amplia lista de capturadoras ya que el mercado actual de capturadoras 4K no está muy poblado.

Enlace: Las mejores capturadoras 4K del mercado que podemos encontrar en Amazon
