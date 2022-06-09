# Clase 13. Instrumentación Científica. Práctica: Detección de Luz

## Instructores

* [Dennis Cazar Ramírez, Universidad San Francisco de Quito (Ecuador)](https://laconga.redclara.net/dennis-cazar/)
* [Harold Yepes Ramírez, Yachay Tech (Ecuador)](https://laconga.redclara.net/harold-yepes-ramirez/)

## Apoyo técnico

* [Jesús Peña Rodríguez, Universidad Industrial de Santander (Colombia)](https://laconga.redclara.net/jesus-pena-rodriguez/)
* [Arturo Sánchez Pineda, Centre National de la Recherche Scientifique (Francia)](https://laconga.redclara.net/arturo-sanchez-pineda/)

## Objetivos de la clase

* Afianzar los fundamentos físicos de la interacción luz-materia, los fundamentos experimentales y la conceptualización alrededor de los sistemas de detección ópticos.
* Profundizar en la comprensión del efecto fotoeléctrico y su aplicación en fotomultiplicadores de tubo de vacío (PMTs) y de arreglos de fotodiodos de avalancha (SiPMs).
* Identificar los principales elementos que componen los bancos de prueba experimentales que se proponen como ejemplos sencillos y prácticos de sistemas de detección de luz en el laboratorio.
* Conectar teoría-experimentación a través de cálculos cortos sobre el papel, asimismo, haciendo uso de una herramienta de simulación en línea para determinar la relación señal-ruido en PMTs y SiPMs, finalizando con un análisis de datos corto, obtenidos con uno de los bancos de prueba experimentales propuestos.

## Material sobre la clase

* [Website de la clase con los fundamentos físicos y bancos de prueba experimentales](https://laconga.redclara.net/courses/modulo-instrumentacion/claseMI13/claseMI13.html)

## ¿En qué consiste la práctica?

La práctica consiste de dos partes de acuerdo a lo revisado en clase y dejado como discusión:

### Parte - I: Calibración del setup con el arreglo de SiPM: Voltaje Umbral ("triggering") y de Polarización

* Voltaje Umbral (Alimentación o "HV" = 1 kV):

    Tenemos el fichero ["calibration_data_trigger-1kv.txt"](Datos/calibration_data_trigger-1kv.txt), con varios niveles de trigger [mV] y las cuentas por minuto [cpm], correspondientes a esta configuración del banco de prueba.

* Voltaje de Polarización:

    Tenemos el fichero ["calibration_data_hv.txt"](Datos/calibration_data_hv.txt), donde se ha variado el HV [V] y se registran las cuentas por minuto [cpm], correspondientes a esta configuración del banco de prueba.

* ¿Que se solicita (tu labor a realizar como entregable) en esta Parte I?

    Graficar y encontrar la zona de plateau (meseta), como óptima región de operación del arreglo de sensores.

### Parte - II: Calibración del setup con PMT: ruido y señal

* Encontraremos en el [repositorio](Datos/) datos crudos (raw) organizados en ficheros (*0V.txt), tomados en una escala de 900-1600V, de los pulsos adquiridos a diferentes valores de HV con trigger de 20mV (es decir, adquisición de todos los datos), la adquisición se llevó a cabo con un osciloscopio a una velocidad de muestreo de 2 GS/s, es decir, 50 ns entre muestra y muestra.

* ¿Que se solicita (tu labor a realizar como entregable) en esta Parte II?

    Escribir un programa para procesar los ficheros y encontrar los picos de cada pulso para producir histogramas de alturas de pico para identificar en que valor de HV los "Dark Pulses" (ruido o pulsos espurios) se diferencian bien de los pulsos de la señal adquirida.

## Indicaciones para la realización y entrega de la práctica

* Disponen de un solo [jupyter notebook](./Practica-deteccion-luz.ipynb) con los datos de calibración cargados para las partes I y II:

    Conéctate a tu cuenta gitlab --> Has un fork de este repositorio --> Clona el fork de tu repositorio en https://jupyter.redclara.net .

* El trabajo se realizará y entregará en grupos de 3 personas:

    Que sea un solo notebook por grupo (que incluya la parte I y II de la práctica) para la corrección, gracias!

## Fecha de entrega

* Jueves, 25 de Marzo de 2021
