# Fuga3D
Repositorio de la impresora "Fuga 3D" del GERUNSJ. Descripción, planos, firmware y archivos de configuración.

Descripción breve. El resto a la wiki.

## Acceso rápido

**Estado actual**: Funcionando.

**Configuraciones**

- ejemplo1: link 1.
- ejemplo2: link2.


## Guía semi-rápida de uso


1. Obtener un modelo 3D. El formato habitual es `.stl`.
    1. Fuentes:
        - [Thingiverse](https://www.thingiverse.com/) , [3DWarehouse](https://3dwarehouse.sketchup.com/) o alternativas
        - ¡Diseñalo! [Autodesk Inventor](https://latinoamerica.autodesk.com/products/inventor/overview) tiene Licencia para estudiantes. Otros: [Freecad](https://www.freecadweb.org/), [Librecad](http://librecad.org), [Sketchup](https://www.sketchup.com/es), [Tinkercad](https://www.tinkercad.com)...
2. Cargar el archivo `.stl` en un programa _slicer_ para generar un archivo `.gcode`, que es el que tiene las instrucciones para la máquina. Sugerimos [Cura](https://ultimaker.com/en/products/cura-software) o [Slic3r](http://www.prusa3d.com/slic3r-prusa-edition/).
    - La impresora tiene un diseño basado en una Prusa i3, así que nuestros perfiles de impresión (o configuración) están basados en eso. Dichos perfiles se encuentran en este repositorio. `ATENCIÓN: estos perfiles funcionarán bien para modelos simples. Para modelos complejos puede ser necesario cambiar algunos parámetros.`
3. Asegurarse de que la impresora está calibrada.
    1. La cama debe estar nivelada. _Lo asumimos como cierto, ya que no debería desnivelarse con el uso._
    2. El origen del eje Z (elevación) debe estar casi pegado a la superficie de la cama (vidrio).
        1. Llevar todos los ejes al origen. Esto define los ceros. `Preparar -> Llevar al Origen`.
        2. Levantar el eje Z un poco: `Preparar -> Mover ejes -> Mover Z -> Girar perilla a la derecha`.
        3. Llevar los ejes X e Y al centro de la cama. La secuencia es similar a la anterior.
        4. Poner un papel debajo del extrusor. Bajar el carro hasta el origen del eje Z: `Preparar -> Origen Z`.
        5. Verificar que el papel quede relativamente apretado. Debe poder deslizarse con cierta dificultad. En caso contrario se debe ajustar el limite del eje Z (final de carrera). Para hacerlo, ajustar o desajustar el tornillo y repetir puntos `d` y `e`.
        6. Una vez calibrada, llevar al origen los ejes (ver punto 1).
4. Cargar el `.gcode` en la memoria SD de la impresora.
5. Aplicar aerosol fijador sobre la superficie del vidrio. ¿Cuánto? Probá. Si se despega la primera capa, te puede haber faltado.
6. Imprimir. `Menu de SD -> Seleccionar el archivo a imprimir`. Una vez seleccionado, la cama empezará a calentar, luego calienta la punta (_hotend_) y finalmente comienza la impresión.

_Sugerencia: el proceso de calentar la cama dura unos 10 minutos; puede ser cómodo precalentarla mientras realizamos el proceso de calibración del eje Z y cargamos los archivos en la tarjeta SD. Hay que tener en cuenta que el aerosol debería colocarse con el vidrio frío, así que es lo primero que puede hacerse._


---------------------

_Grupo Estudiantil de Robótica de la Universidad Nacional de San Juan_
