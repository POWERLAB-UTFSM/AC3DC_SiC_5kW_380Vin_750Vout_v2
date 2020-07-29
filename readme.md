# AC3DC_SiC_5kW_380Vin_750Vout_v2

## Resumen
Este repositorio corresponde al diseño de un rectificador trifásico boost de dos niveles de 5kW, con una tensión de salida de 750VDC, una tensión de entrada entre líneas de 380VAC, y operado usando SiC MOSFETs

## Pertenencia a proyecto
* **Código Proyecto**: FONDEF IT 18I0090
* **Título Proyecto**: 
* **Investigadores responsables**:
    * Ana Llor (Directora)
    * Freddy Flores
    * Marcelo Pérez
    * Samir Kouro
    * Alan Wilson
    * Sebastián Rivera
* **Estado**: En desarrollo
* **Inicio**: Junio 2019
* **Término**: -

## Autores del repositorio
* Leonardo Solís
* Alan Wilson 

## Ramas del repositorio
* master

## Sub-Carpetas
1. `SUBBOARD-phase_leg_3p_2L`: Proyecto con la placa de la etapa de las piernas del rectificador, incluyendo el Dc-link.
1. `SUBBOARD-boost_filter_3p_LCL`: Proyecto con la placa del filtro trifásico LCL de entrada.
1. `SUBBOARD-gate_driver`: Proyecto con la placa del gate driver para disparar los MOSFETs de la etapa de potencia.
1. `SUBBOARD-power_sources`: Proyecto con la placa de la fuente auxlilar que alimenta el convertidor desde los 380VAC.
1. `SUBBOARD-current_measurement`: Proyecto con la placa de medición de corriente.
1. `SUBBOARD-voltage_sensors`: Proyecto con la placa de sensores de voltaje diferencial de alta impedancia
1. `MULTIBOARD-project`: Ensamblado 3D de las placas.
1. `AUXFILES`: Archivos auxiliares.

## Software para modificar repositorio
* Altium Designer (v.20)

## Detalles técnicos del diseño
| **Descripción** | **Tipo** |
| - | - |
| Convertidor | AC3p-DC | 
| Topología | boost de 2 niveles | 
| Aislación Galvánica | No | 
| Potencia nominal | 5000 W | 
| Tensión de entrada nominal | 380 V AC | 
| Semiconductores de potencia | SiC MOSFET | 
| Control | Microcontrolador embebido (c2000 - Texas Instruments) | 

## Usar Git con este proyecto
Para descargar este proyecto al computador local:
1. Instalar Git: https://git-scm.com/downloads
1. Instalar Git LFS: https://git-lfs.github.com/
1. Inicializar Git LFS:<br />
`git lfs install`
1. Ir al directorio principal donde se quiere dejar el repositorio local, y clonar desde el repositorio remoto `https://remote.git`:<br />
`git clone https://remote.git` <br />
En este caso: <br />
`git clone https://github.com/POWERLAB-UTFSM/DCDC_SiC_600W_750Vdcin_v1p1.git`

### Usar Git en Altium
1. **Save:** Una vez que los cambios se hayan efectuado, guarda el archivo o proyecto.
1. **Commit:** Clock derecho en el archivo o proyecto, luego `Version Control` -> `Commit`. Añane una nota con los cambios hechos. Los cambios permanecerán en el repositorio local hasta que no se suban los cambios con el siguiente comando.
1. **Push:** Cuando se quiere subir al repositorio remoto todos los cambios efectuados, click derecho en el archivo o proyecto, luego `Version Control` -> `Push`.
1. **Check:** Verifica que todo se ha subido correctamente al repositorio remoto.

Para más información: https://www.altium.com/documentation/altium-designer/using-version-control-ad

### Usar Git desde la línea de comandos (manual)
1. **Abrir Bash:** <br /> Una vez que se hayan hecho las actualizaciones, ve al directorio del proyecto, abre la ventana de comandos de Git (Git Bash, u otro) y ejecuta:
1. `git status` <br /> Muestra los cambios hechos.
1. `git add [path/file]` <br /> Prepara los archivos/carpetas efectivos para consolidar (**Commit**). Para añadir todos los archivos a la vez, ejecutar `git add .`.
1. `git commit -m "description"` <br /> Consolida los cambios hechos con su respectiva descripción, y agrega el comentario `description`.
1. `git push origin master` <br /> Sube los cambios desde el repositorio local `origin` y la rama `master`, al repositorio remoto. Cambiar el nombre del repositorio local y rama, de ser necesario.
1. `git pull origin master` <br /> Descarga los últimos cambios desde el repositorio remoto hacia el repositorio local `origin` y la rama `master`.

Para más información: https://git-scm.com/doc

## Otros comentarios
