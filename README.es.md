# MemoryCleaner

**Limpiador de memoria ligero y gratuito para Windows: libera memoria con un clic y limpia solo según las condiciones que usted fije.**

[English](README.md) · [한국어](README.ko.md) · [简体中文](README.zh-CN.md) · [日本語](README.ja.md) · Español · [Português (Brasil)](README.pt-BR.md) · [Français](README.fr.md)

> Este documento es una traducción. Si hay alguna diferencia, la [versión en coreano](README.ko.md) es la que prevalece.

![Platform](https://img.shields.io/badge/platform-Windows%2010%20%2F%2011%20(64--bit)-0078D4)
![License](https://img.shields.io/badge/license-Freeware-brightgreen)
![Version](https://img.shields.io/badge/version-3.0.0-blue)
[![Download](https://img.shields.io/badge/download-kilho.net-orange)](https://down.kilho.net/memorycleaner?lang=es)

![Pantalla de MemoryCleaner](images/memorycleaner-en.webp)

## Descripción general

MemoryCleaner muestra cuánta memoria se está usando en este momento y, con un solo clic en **Limpiar memoria**, recupera la caché que Windows mantiene reservada y la memoria que los programas abiertos no están usando ahora.

Puede configurarlo para que limpie solo cuando el uso de memoria sea alto, a intervalos fijos o cuando la caché se acumule y falte memoria libre. Mientras un juego o un vídeo se ejecuta a pantalla completa, se salta la limpieza para no molestar.

Al cerrar la ventana pasa al área de notificación (bandeja del sistema), donde sigue trabajando en silencio. Cuando la ventana se cierra, MemoryCleaner libera también toda la memoria que ella usaba, así que mientras espera en la bandeja solo ocupa alrededor de 1 MB.

## Funciones principales

- **Limpieza con un clic** — Limpie la memoria con el botón **Limpiar memoria** o con un solo clic en el icono de la bandeja.
- **Elegir qué limpiar** — Elija usted mismo las áreas: caché de archivos, conjunto de trabajo, lista de espera, caché del registro, combinar memoria y más.
- **Limpieza automática** — Limpia cuando el uso de la memoria física · virtual · del conjunto de trabajo supera un umbral, o a intervalos fijos.
- **Anti-tirones en juegos** — Cuando la caché (la lista de espera) se acumula y falta memoria libre, vacía solo la caché.
- **Detección de pantalla completa** — Se salta la limpieza automática mientras un juego, vídeo o presentación está a pantalla completa.
- **Estado de la memoria** — Vea la memoria física, la virtual, el conjunto de trabajo y la caché en la pantalla de inicio y en el icono de la bandeja.
- **Ligero** — Un solo ejecutable que ocupa alrededor de 1 MB mientras espera en la bandeja.
- **9 idiomas** — Coreano · inglés · japonés · chino · ruso · italiano · francés · español · árabe.

## Descarga / Instalación

| Tipo | Enlace |
|---|---|
| Instalador | [Descargar](https://down.kilho.net/memorycleaner?lang=es) |
| Portátil (ZIP) | [Descargar](https://down.kilho.net/memorycleaner?lang=es&nosetup) |

El instalador abre MemoryCleaner en cuanto termina la instalación y activa **Ejecutar al iniciar el sistema**, así que se inicia en la bandeja cada vez que inicia sesión en Windows. Para la versión portátil, descomprima el ZIP y ejecute `MemoryCleaner.exe`. Las dos versiones tienen las mismas funciones.

Limpiar la memoria requiere permisos de administrador, por lo que Windows muestra una solicitud de permiso al ejecutarlo. Pulse **Sí**.

## Uso

### Primeros pasos

1. Ejecute MemoryCleaner y pulse **Sí** en la solicitud de permisos de administrador.
2. **Inicio** muestra el uso de la memoria física como barra y cifras, y debajo la memoria virtual · el conjunto de trabajo · la caché. Los valores se actualizan cada segundo.
3. Pulse **Limpiar memoria**: el botón cambia a **Limpiando** y, al terminar, verá enseguida que el uso ha bajado.
4. Para que limpie solo, pulse **Configurar** y active las condiciones que quiera en **Limpieza automática**.
5. Al cerrar la ventana, MemoryCleaner sigue funcionando en la bandeja. Haga clic en el icono para volver a abrir la ventana.

### Distribución de la pantalla

**Botones superiores**

| Elemento | Función |
|---|---|
| **Inicio** | La pantalla principal, con el estado de la memoria y el botón **Limpiar memoria** |
| **Configurar** | Limpieza automática · Áreas a limpiar · General |
| **Donar** | Abre la página de donaciones |
| Logotipo de KILHO.net | Abre la página de presentación de MemoryCleaner |

**Inicio**

| Elemento | Contenido |
|---|---|
| Barra | Uso de la memoria física |
| **física** | Usada / total (MB) y porcentaje de uso |
| **virtual** | Uso de la memoria virtual, incluido el archivo de paginación |
| **Trabajo** | Memoria ocupada por los programas abiertos y su proporción |
| **Caché** | Memoria que Windows mantiene como caché (el mismo valor que «En caché» en el Administrador de tareas) y su proporción respecto a la memoria física |
| **Limpiar memoria** | Limpia ahora mismo. Cambia a **Limpiando** mientras trabaja |

**Configurar**

| Grupo | Elementos |
|---|---|
| **Limpieza automática** | **Limpiar cuando uso de memoria física es mayor que (%)** · **Limpiar cuando uso archivo paginación es mayor que (%)** · **Limpiar cuando uso total del conj. trabajo es superior al (%)** · **Limpiar automáticamente si se excede intervalo (minutos).** · **Vaciar la caché (lista de espera) (anti-tirones)** · **No limpiar en pantalla completa** |
| **Áreas a limpiar** | **Caché de archivos** · **Trabajo** · **Lista de espera (baja prioridad)** · **Caché del registro** · **Combinar memoria** · **Lista de espera \*** · **Lista de páginas modificadas \*** |
| **General** | **Ejecutar al iniciar el sistema** · **Limpiar con clic en icono de la tarea** |
| Abajo | Versión actual y botón **Predeterminados** |

**Icono de la bandeja**

| Acción | Resultado |
|---|---|
| Pasar el ratón | Uso de la memoria física · virtual · del conjunto de trabajo |
| Clic izquierdo | Abre la ventana (limpia al momento si **Limpiar con clic en icono de la tarea** está activado) |
| Clic derecho | **Limpiar memoria** (abrir la ventana) · **Elaborado por Kilho** (página de presentación) · **Salir** |

Mientras limpia, el icono de la bandeja cambia de aspecto, así que sabe que está trabajando sin abrir la ventana.

**Áreas a limpiar** — qué libera cada una

| Elemento | Qué libera | Predeterminado |
|---|---|---|
| **Caché de archivos** | La caché que Windows acumula al leer y escribir archivos | Activado |
| **Trabajo** | La memoria que los programas abiertos no están usando ahora | Activado |
| **Lista de espera (baja prioridad)** | La parte de la caché con menos probabilidades de volver a usarse | Activado |
| **Caché del registro** | La caché acumulada al leer el registro | Activado |
| **Combinar memoria** | Une en una sola los contenidos de memoria idénticos para liberar espacio | Activado |
| **Lista de espera \*** | Toda la caché | Desactivado |
| **Lista de páginas modificadas \*** | La memoria que espera ser escrita en disco | Desactivado |

Los elementos marcados con `*` pueden provocar tirones breves en juegos o al reproducir vídeo, por eso vienen desactivados.

### Qué hacer cuando…

**Quiere limpiar la memoria ahora mismo**
Pulse **Limpiar memoria** en **Inicio**. Mientras trabaja, el botón cambia a **Limpiando** y al terminar vuelve a **Limpiar memoria**. Púlselo cuando el PC vaya pesado tras tener muchos programas abiertos mucho tiempo, o justo antes de abrir un juego grande o un programa de edición.

**Quiere limpiar desde el icono de la bandeja sin abrir la ventana**
Active **Configurar → Limpiar con clic en icono de la tarea** y un solo clic en el icono de la bandeja limpiará la memoria. Al terminar aparece la notificación «Memoria optimizada.». Mientras este ajuste esté activado, abra la ventana con clic derecho en el icono → **Limpiar memoria**.

**Quiere ver el estado de la memoria sin la ventana**
Pase el ratón sobre el icono de la bandeja para ver el uso de la memoria física · virtual · del conjunto de trabajo: suficiente para saber si hace falta limpiar sin abrir la ventana.

**Quiere que limpie solo cuando falte memoria**
En **Configurar → Limpieza automática**, active **Limpiar cuando uso de memoria física es mayor que (%)** y elija un umbral (30 – 90 %) en la casilla de al lado. Cuando el uso supere el umbral, MemoryCleaner limpiará solo. Si usa mucho el archivo de paginación, active también **Limpiar cuando uso archivo paginación es mayor que (%)**; si el problema son los programas que acaparan memoria, active **Limpiar cuando uso total del conj. trabajo es superior al (%)**. Cuando la limpieza no baja el uso, espera antes de volver a limpiar en lugar de hacerlo una y otra vez, para que la limpieza no se convierta en una carga.

**Quiere limpiar a intervalos regulares**
Active **Limpiar automáticamente si se excede intervalo (minutos).** y elija 5 · 10 · 20 · 30 · 40 · 50 · 60 minutos: limpiará con ese intervalo sin importar el uso. Útil para mantener ligero un PC que pasa mucho tiempo encendido.

**Un juego va cada vez más a tirones cuanto más juega (vaciar la caché)**
A veces un juego da cada vez más tirones con el tiempo, hasta que solo se arregla reiniciándolo. Se debe a que Windows guarda como caché (la lista de espera) los archivos que ya ha leído; cuando esa caché se acumula y la memoria libre se agota, Windows tiene que recuperarla a toda prisa y el juego se congela un instante. Active **Vaciar la caché (lista de espera) (anti-tirones)**: cuando la caché supere el umbral **Vaciar si la caché (MB) supera** (512 · 1024 · 2048 · 4096 MB) y a la vez la memoria libre baje del umbral **Vaciar si la memoria libre (MB) es menor que** (1024 · 2048 · 4096 · 8192 · 16384 MB), vaciará solo la caché por adelantado. Solo actúa cuando se cumplen las dos condiciones, y al vaciarla estas desaparecen solas, así que solo interviene cuando hace falta.

Lo recomendable es fijar el umbral de memoria libre en la mitad de la memoria instalada en su PC.

| Memoria instalada | Vaciar si la memoria libre (MB) es menor que |
|---|---|
| 8 GB | 4096 (predeterminado) |
| 16 GB | 8192 |
| 32 GB | 16384 |

No hace falta activarlo solo para jugar. Ocupa alrededor de 1 MB en la bandeja y solo actúa cuando se cumplen las condiciones, así que puede dejarlo activado.

**Quiere que no toque nada durante un juego o una película**
**No limpiar en pantalla completa** viene activado. Mientras un juego, vídeo o presentación está a pantalla completa, se salta la limpieza automática para evitar tirones. Al salir de la pantalla completa, vuelve a funcionar con normalidad.

**Quiere elegir usted qué áreas limpiar**
Marque las áreas a limpiar en **Configurar → Áreas a limpiar**. Tanto el botón **Limpiar memoria** como la limpieza automática siguen esta selección. Si no marca ninguna, no hay nada que hacer y el botón **Limpiar memoria** aparece atenuado.

**Quiere una limpieza más a fondo**
Al activar **Lista de espera \*** y **Lista de páginas modificadas \*** se libera también toda la caché y la memoria que espera ser escrita, que es lo que más memoria libera. Aun así, puede provocar tirones breves en juegos o vídeos, así que actívelos solo cuando lo necesite y déjelos desactivados el resto del tiempo.

**Quiere saber qué significa «Caché»**
**Caché** en **Inicio** es la memoria que Windows guarda por si vuelve a necesitarla: el mismo valor que «En caché» en el Administrador de tareas. Un valor alto no es malo en sí, pero si los juegos dan tirones, pruebe a activar el vaciado de la caché de arriba.

**Quiere que se inicie con Windows**
Active **Configurar → Ejecutar al iniciar el sistema** y, poco después de iniciar sesión en Windows, MemoryCleaner se iniciará en silencio en la bandeja, sin solicitud de permisos de administrador. En la versión instalada ya viene activado.

**Quiere que siga funcionando tras cerrar la ventana**
La X de la ventana no cierra MemoryCleaner: pasa a la bandeja y sigue con la limpieza automática. Además libera toda la memoria que usaba la ventana, así que dejarlo en marcha apenas cuesta nada. Para salir del todo, haga clic derecho en el icono de la bandeja → **Salir** y confirme.

**Sale mientras está limpiando**
Si sale mientras hay una limpieza en curso, el botón cambia a **Salir después de limpiar** y el programa se cierra al terminar la limpieza. La limpieza nunca se corta a medias.

**Quiere volver a la configuración inicial**
Pulse **Predeterminados** en la parte inferior de **Configurar** y confirme: todos los ajustes de limpieza automática y de áreas a limpiar vuelven a sus valores predeterminados. **Ejecutar al iniciar el sistema** no se modifica.

**Lo ejecuta de nuevo cuando ya está en marcha**
Solo funciona un MemoryCleaner a la vez. Si lo ejecuta de nuevo mientras está en la bandeja, no se abre otro: se abre la ventana del que ya está en marcha.

## Configuración

Cada ajuste se guarda en cuanto lo cambia y se vuelve a usar en el próximo inicio.

| Elemento | Valor predeterminado |
|---|---|
| Limpieza según el uso de la memoria física · archivo de paginación · conjunto de trabajo | Desactivado (umbral del 90 % al activarlo) |
| Limpiar automáticamente si se excede intervalo (minutos). | Desactivado (30 minutos al activarlo) |
| Vaciar la caché (lista de espera) | Desactivado (caché ≥ 1024 MB · memoria libre < 4096 MB al activarlo) |
| No limpiar en pantalla completa | Activado |
| Áreas a limpiar | Caché de archivos · Trabajo · Lista de espera (baja prioridad) · Caché del registro · Combinar memoria |
| Ejecutar al iniciar el sistema | Activado en la versión instalada |
| Limpiar con clic en icono de la tarea | Desactivado |
| Idioma | Sigue la configuración regional de Windows (inglés si el idioma no está disponible) |

## Requisitos

- Windows 10 · Windows 11 (64 bits)
- Permisos de administrador: necesarios para limpiar la memoria. Aparece una solicitud al ejecutarlo (pero no cuando se inicia con **Ejecutar al iniciar el sistema**).
- No hay que instalar ningún otro componente.
- La conexión a Internet solo se usa para avisar de nuevas versiones.

## Actualizaciones

MemoryCleaner **no** se actualiza solo. Al iniciarse comprueba si hay una versión nueva y muestra un aviso; al hacer clic en **[Sí]** abre la página de descarga y cierra el programa. Las versiones nuevas se publican manualmente tras pruebas internas y se anuncian en la [página de MemoryCleaner](https://kilho.net/memorycleaner). Consulte el [aviso sobre la política de actualizaciones](https://en.kilho.net/archives/notice/2940).

**Historial de versiones**

| Versión | Fecha | Cambios |
|---|---|---|
| 3.0.0 | 2026-09-29 | Rehecho por completo en C puro, más rápido y estable: memoria en espera en la bandeja reducida más de un 95 % y tamaño del programa alrededor de un 98 %, elección de las áreas a limpiar, vaciado automático de la caché (anti-tirones en juegos), caché mostrada en la pantalla de inicio, ajustes de limpieza predeterminados pensados para juegos y vídeo, botón para restaurar los valores predeterminados, comprobación de actualizaciones e inicio más fiables |
| 2.0.3 | 2026-09-03 | Mejor detección de pantalla completa para no interrumpir juegos y vídeos, cierre más estable, avisos de fin de limpieza más precisos, limpiezas repetidas optimizadas, ajustes más estables |
| 2.0.2 | 2026-08-13 | Opción para saltarse la limpieza a pantalla completa, el inicio automático se elimina al desinstalar, carga de ajustes e inicio automático más fiables |
| 2.0.1 | 2026-07-13 | Limpieza de memoria de navegadores reforzada, más estabilidad en sesiones largas, avisos y ajustes más fiables, se añade el español |

## Licencia

MemoryCleaner es **freeware**. Puede usarlo gratis y sin restricciones en cualquier lugar —en la empresa, en casa, en organismos públicos o en centros educativos— y redistribuirlo libremente.

## Enlaces

- Sitio web: <https://kilho.net/memorycleaner>
- Foro: <https://groups.google.com/g/kilhonet>
- X (Twitter): <https://www.twitter.com/kilhonet>

© KILHO.NET
