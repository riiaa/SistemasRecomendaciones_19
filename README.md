# Sistemas de Recomendaciones @ RIIAA '19
Este repositorio contiene el material relacionado con el taller (workshop) de "Sistemas de Recomendaciones" dentro de la RIIAA '19. El taller se enfocará en entender la importancia de los sistemas de recomendaciones, la formulación del problema de predicción, y las técnicas más importantes del área. También se explorarán algunos temas de investigación de este área.
Además de los Jupyter Notebooks que se encuentran en este repositorio, se utilizarán unas diapositivas en Google Slides (https://docs.google.com/presentation/d/1Ps63of3KEXU8c249WGadP9ogFhhrp0_pPZq6AJTcUj4/edit?usp=sharing) para presentar varios conceptos y fórmulas.

# Datos
Los datos que se utilizaron para este taller originan de la base de datos MovieLens (https://grouplens.org/datasets/movielens/).

# Instrucciones para estudiantes

La mayoría de las prácticas de los talleres se desarrollarán en Python 3.7+ usando la biblioteca [Tensorflow 2.0](https://www.tensorflow.org/), que adopta [Keras](https://www.tensorflow.org/versions/r2.0/api_docs/python/tf/keras) como interfaz de alto nivel para construir y entrenar redes neuronales.

Cosas para preparar
* Una laptop.
* Este repositorio de GitHub clonado y actualizado antes del taller.
* Un sentido aventurero en los datos.
* Un ambiente Python 3.7+ con Anaconda (ver opciones 1 y 2 abajo).

Los talleres serán impartidos usando *notebooks* de Jupyter, documentos con código ejecutable, texto, ecuaciones, visualizaciones, imágenes y demás material. Los *notebooks* se pueden crear y ejecutar en la nube vía Google Colab (opción 1) o de manera local en tu computadora a través de [Jupyter Notebooks](https://jupyter.org/) (opción 2).

### Opcion 1: Google Colab
[Colab](https://colab.research.google.com) es un servicio de Google para ejecutar *notebooks* en la nube. Provee ambientes de Python 2 y 3 con CPUs, GPUs y TPUs. ¡Y es gratis! Solo necesitas tener una cuenta de Google o crear una.

Recomendamos que elijas un ambiente con Python 3 y GPU. Para activarlo:
* Abre el menú `Entorno de ejecución`
* Elige la opción `Restablecer todos los entornos de ejecución...` .
* Vuelve a abrir `Entorno de ejecución`
* Elige `Cambiar tipo de entorno de ejecución`
* Selecciona Python 3 como `Tipo de ejecución` y GPU de la lista de `Acelerador por hardware`

La siguiente captura de pantalla ilustra este proceso.

![](media/escoge_acelerador.png)

En [Colab](https://colab.research.google.com) puedes crear un nuevo *notebook*, subir uno existente desde tu computadora o importarlo de Google Drive o GitHub.

### Opcion 2: Ambiente local
Para tener la versión de Python 3.7+ y todas las bibliotecas instaladas en cualquier plataforma, recomendamos que uses [**Anaconda**](https://www.anaconda.com/) y generes un ambiente con el archivo `environment.yml` de este repositorio usando una terminal y el comando:

```
conda env create -n riiaa19 -f environment_cpu.yml
```

Cambia el nombre `riia19` por tu nombre favorito para el ambiente. Si cuentas con un GPU Nvidia y deseas aprovecharlo cambia el archivo `environment_cpu.yml` a `environment_gpu.yml`.

Para activar el ambiente que creaste, en una terminal ingresa el comando

```
conda activate riiaa19
```

Una vez activado, puedes ejecutar la aplicación de Jupyter Notebook

```
jupyter notebook
```

Este comando abrirá una pestaña o ventana en tu navegador web, como se muestra en la siguiente captura de pantalla:

![](media/jupyter_notebook.png)

Al igual que en Google Colab, puedes crear un nuevo *notebook* seleccionando el botón `New` y posteriormente `Python 3`. De forma alternativa, puedes abrir uno existente seleccionando el archivo del *notebook* (con extensión `.ipynb`) dentro del directorio donde ejecutaste Jupyter Notebook. Con el botón `Upload` agregas archivos que se encuentran en otra parte de tu computadora a este directorio. Para cerrar Jupyter Notebook, presiona el botón `Quit` y posteriormente cierra la pestaña o ventana de tu navegador web.

Para desactivar el ambiente `riiaa19` de Anaconda simplemente haz

```
conda deactivate
```
