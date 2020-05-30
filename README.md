# Desmenuzando a las neuronas artificiales

![GitHub last commit](https://img.shields.io/github/last-commit/QuarantineHUB/desmenuzando-nns?style=for-the-badge) 
![GitHub repo size](https://img.shields.io/github/repo-size/QuarantineHUB/desmenuzando-nns?style=for-the-badge) 
![License](https://img.shields.io/github/license/RodolfoFerro/PyConCo20?style=for-the-badge) 
[![Twitter](https://img.shields.io/twitter/follow/FerroRodolfo?label=Twitter&logo=twitter&style=for-the-badge)](https://twitter.com/FerroRodolfo/) 
[![LinkedIn](https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555)](https://www.linkedin.com/in/rodolfoferro/) 
- Presentación: [![Slides](https://img.shields.io/static/v1?label=Slides&message=Google%20Slides&color=tomato)](https://docs.google.com/presentation/d/e/2PACX-1vSTSwM0Mvf2Hr4CZzc__z7_Muaij3cHzpsq6B8qnM3FLlnUrpwk6NDN68LYRQt8BLjLqni1O8_3WXk8/pub?start=false&loop=false&delayms=3000)
- Cuaderno de trabajo: [![Sin resolver](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/QuarantineHUB/desmenuzando-nns/blob/master/notebooks/Desmenuzando%20a%20las%20neuronas%20artificiales%20(Sin%20resolver).ipynb)
- Cuaderno resuelto: [![Resuelto](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/QuarantineHUB/desmenuzando-nns/blob/master/notebooks/Desmenuzando%20a%20las%20neuronas%20artificiales%20(Resuelto).ipynb)

Este repositorio de GitHub contiene el material de la ponencia "Desmenuzando a las neuronas artificiales" por Rodolfo Ferro, para el [Programmathon 2020](https://quarantinehub.github.io/).

#### ¿Nunca has usado GitHub, Markdown o Jupyter/Google Colab?

Hay muchas guías en línea para usar estas tecnologías, algunas recomendaciones:
- GitHub: https://guides.github.com/activities/hello-world/.
- Markdown: https://guides.github.com/features/mastering-markdown/.
- Notebooks: 
  - Jupyter: https://jupyter.org/
  - Nbviewer: https://nbviewer.jupyter.org/github/jupyter/notebook/tree/master/docs/source/examples/Notebook/
  - Google Colab: https://colab.research.google.com
  - Azure notebooks: https://notebooks.azure.com/

**¿Tienes más dudas?** Escríbele a los organizadores o abre un [issue](https://help.github.com/en/articles/creating-an-issue).

## Organización del repositorio

La estructura está inspirada en una versión lite de [cookie cutter data science project](https://drivendata.github.io/cookiecutter-data-science/):

- `notebook/`: Notebooks que se pueden lanzar en colab (o la plataforma que hayas definido). Enumera los notebook en orden de uso.
- `media/`: Imágenes, PDFs y demás material de media para usar en tus notebooks y repo.
- `README.md`: Archivo Markdown de entrada para la página y tu ponencia.

## ¿Sugerencias? ¿Mejoras?
Manda un [pull request](https://help.github.com/en/articles/about-pull-requests), lo evaluaremos, empezaremos una discusion y si es buena idea lo incorporaremos. :100:

## Instrucciones para asistentes

**_Las siguientes instrucciones se pueden copiar para tu ponencia._**

La mayoría de las sesiones prácticas se desarrollarán en Python 3.7+, por lo que a continuación te compartimos la manera en la que puedes preparar tu entorno.

Cosas para preparar:
- Una laptop.
- Este repositorio de GitHub clonado y actualizado antes de la ponencia.
- Un sentido aventurero en los datos y la programación.
- Un ambiente Python 3.7+ con Anaconda (ver opciones 1 y 2 abajo).

Las ponencias serán impartidocompartidass usando *notebooks* de Jupyter, documentos con código ejecutable, texto, ecuaciones, visualizaciones, imágenes y demás material. Los *notebooks* se pueden crear y ejecutar en la nube vía Google Colab (opción 1) o de manera local en tu computadora a través de [Jupyter Notebooks](https://jupyter.org/) usando Anaconda (opción 2).

### Opción 1: Google Colab

[Google Colab](https://colab.research.google.com) es un servicio de Google para ejecutar *notebooks* en la nube. Provee ambientes de Python 2 y 3 con CPUs, GPUs y TPUs. ¡Y es gratis! Sólo necesitas tener una cuenta de Google o crear una.

Recomendamos que elijas un ambiente con Python 3 y GPU para tu ponencia. Para activarlo:
- Abre el menú `Entorno de ejecución`
- Elige la opción `Restablecer todos los entornos de ejecución...`
- Vuelve a abrir `Entorno de ejecución`
- Elige `Cambiar tipo de entorno de ejecución`
- Selecciona Python 3 como `Tipo de ejecución` y GPU de la lista de `Acelerador por hardware`

La siguiente captura de pantalla ilustra este proceso.
![](media/escoge_acelerador.png)

En [Google Colab](https://colab.research.google.com) puedes crear un nuevo *notebook*, subir uno existente desde tu computadora o importarlo de Google Drive o GitHub.

### Opción 2: Ambiente local

Para tener la versión de Python 3.7+ y todas las bibliotecas instaladas en cualquier plataforma, recomendamos que uses [**Anaconda**](https://www.anaconda.com/) y generes un ambiente con el archivo `environment.yml` de este repositorio usando una terminal y el comando:

```
conda env create -n qhub -f environment_cpu.yml
```

Cambia el nombre `qhub` por tu nombre favorito para el ambiente. Si cuentas con un GPU Nvidia y deseas aprovecharlo cambia el archivo `environment_cpu.yml` a `environment_gpu.yml`.

Para activar el ambiente que creaste, en una terminal ingresa el comando

```
conda activate qhub
```

Una vez activado, puedes ejecutar la aplicación de Jupyter Notebook

```
jupyter notebook
```

Este comando abrirá una pestaña o ventana en tu navegador web, como se muestra en la siguiente captura de pantalla:
![](media/jupyter_notebook.png)

Al igual que en Google Colab, puedes crear un nuevo *notebook* seleccionando el botón `New` y posteriormente `Python 3`. De forma alternativa, puedes abrir uno existente seleccionando el archivo del *notebook* (con extensión `.ipynb`) dentro del directorio donde ejecutaste Jupyter Notebook. Con el botón `Upload` agregas archivos que se encuentran en otra parte de tu computadora a este directorio. Para cerrar Jupyter Notebook, presiona el botón `Quit` y posteriormente cierra la pestaña o ventana de tu navegador web.

Para desactivar el ambiente `qhub` de Anaconda simplemente ejecuta:
```
conda deactivate
```

## Atribuciones

Este repositorio está construido a partir de la plantilla creada para la Reunión Internacional de Inteligencia Artifical y sus Aplicaciones (RIIAA), que puedes encontrar [aquí](https://github.com/riiaa/riiaa19_workshop_template).
