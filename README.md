# Geological Modeling of the Los Santos Formation / Modelo Geológico de la Formación Los Santos

[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)
[![GemPy](https://img.shields.io/badge/GemPy-2.3.1-blue)](https://www.gempy.org/)

## English

This repository contains the data and results of the 3D geological modeling of the Los Santos Formation, developed as part of the thesis:

> *3D Geological Modeling of the Los Santos Formation to Strengthen the Hydrogeological Model of the Mesa de los Santos (Santander) Using Open-Source Tools*

The modeling was carried out using [GemPy](https://www.gempy.org/) 2.3.1, a free and open-source Python library for implicit 3D geological modeling.

### Repository Structure

​```
data/
        regional/
            surfaces_regional.txt
            orientations_regional.txt
        detail/
            surfaces_detail.txt
            orientations_detail.txt
    output/
        regional_model.vtkjs
        detail_model.vtkjs
    figures/
        regional_model.png
        detail_model.png
    README.md
    LICENSE
    environment.yml
    
​```

### Results

| Regional Model | Detail Model |
|---------------|--------------|
| ![Regional Model](figures/regional_model.png) | ![Detail Model](figures/detail_model.png) |

### How to visualize the VTK files

The `.vtk` files can be opened with [ParaView](https://www.paraview.org/), a free and open-source visualization software.

1. Download and install ParaView from [paraview.org](https://www.paraview.org/)
2. Open ParaView and go to `File > Open`
3. Select the `.vtk` file
4. Click `Apply` in the Properties panel

### How to reproduce the models

1. Clone this repository
2. Install the environment:
​```bash
conda env create -f environment.yml
conda activate gempy_env
​```
3. Load the data files into GemPy following the [official documentation](https://docs.gempy.org/)

### Citation

If you use this data or results, please cite:

> Sánchez-Mateus, A.F. & Duarte-Guevara, E.M. (2025). *3D Geological Modeling of the Los Santos Formation to Strengthen the Hydrogeological Model of the Mesa de los Santos (Santander) Using Open-Source Tools*. Universidad Industrial de Santander.
> Supervisors: Velandia-Patiño, F.A. & Cetina-Tarazona, M.A.

---

## Español

Este repositorio contiene los datos y resultados del modelamiento geológico 3D de la Formación Los Santos, desarrollado como parte de la tesis:

> *Modelado Geológico 3D de la Formación Los Santos Para Fortalecer el Modelo Hidrogeológico de la Mesa de los Santos (Santander) Usando Herramientas de Libre Acceso*

El modelamiento fue realizado con [GemPy](https://www.gempy.org/) 2.3.1, una librería de Python de libre acceso para modelamiento geológico 3D implícito.

### Estructura del repositorio

​```
├── data/
│   ├── regional/
│   │   ├── surfaces_regional.txt      # Puntos de superficies - modelo regional
│   │   └── orientations_regional.txt  # Datos de orientaciones - modelo regional
│   └── detail/
│       ├── surfaces_detail.txt        # Puntos de superficies - modelo de detalle
│       └── orientations_detail.txt    # Datos de orientaciones - modelo de detalle
├── output/
│   ├── regional_model.vtk             # Modelo regional (3D)
│   └── detail_model.vtk               # Modelo de detalle (3D)
└── figures/
    ├── regional_model.png
    └── detail_model.png
​```

### Resultados

| Modelo Regional | Modelo de Detalle |
|----------------|-------------------|
| ![Modelo Regional](figures/regional_model.png) | ![Modelo de Detalle](figures/detail_model.png) |

### Cómo visualizar los archivos VTK

Los archivos `.vtk` pueden abrirse con [ParaView](https://www.paraview.org/), un software de visualización gratuito y de código abierto.

1. Descarga e instala ParaView desde [paraview.org](https://www.paraview.org/)
2. Abre ParaView y ve a `File > Open`
3. Selecciona el archivo `.vtk`
4. Haz clic en `Apply` en el panel de propiedades

### Cómo reproducir los modelos

1. Clona este repositorio
2. Instala el entorno:
​```bash
conda env create -f environment.yml
conda activate gempy_env
​```
3. Carga los archivos de datos en GemPy siguiendo la [documentación oficial](https://docs.gempy.org/)

### Citación

Si usas estos datos o resultados, por favor cita:

> Sánchez-Mateus, A.F. & Duarte-Guevara, E.M. (2025). *Modelado Geológico 3D de la Formación Los Santos Para Fortalecer el Modelo Hidrogeológico de la Mesa de los Santos (Santander) Usando Herramientas de Libre Acceso*. Universidad Industrial de Santander.
> Directores: Velandia-Patiño, F.A. & Cetina-Tarazona, M.A.
