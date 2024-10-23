# Seminario: Modelos Fundacionales (SAM y CLIP)

Este repositorio contiene notebooks para aplicar y explorar modelos fundacionales de imágenes, como **CLIP** y **SAM (Segment Anything Model)**. A continuación se detallan los pasos para configurar el entorno y ejecutar los notebooks correspondientes.

## Requisitos previos

Antes de empezar, asegúrate de tener instalados los siguientes programas en tu sistema:

- Python 3.10 o superior
- Visual Studio Code (VSCode)
- Poetry (se instalará en el proceso)

## Clonar el Repositorio

Primero, clona el repositorio en tu máquina local:

```bash
git clone https://github.com/marma18m/seminario-foundation-models.git
cd seminario-foundation-models
```

## Configuración del Entorno

### Crear y activar un entorno virtual para cada modelo

Primero, debes crear un entorno virtual e instalar las dependecias de sam

```bash
cd seminario-foundation-models/sam
python -m venv .sam
source .sam/bin/activate

pip install --upgrade pip
pip install poetry

poetry install
```

Configuramos el kernel en vscode, para eso

- ctrl + shif + p -> reload window

Si cuando le dais a selecicionar kernel de un python env no os sugiere el que toca:

```bash
python -m ipykernel install --user --name=.sam --display-name="SAM"
```

- ctrl + shif + p -> reload window

Cuando ya esté seleccionado, deseactivamos el envirnoment --> deactivate

Luego lo haremos con el de CLIP:

```bash
cd seminario-foundation-models/faiss
python -m venv .faiss
source .faiss/bin/activate
pip install --upgrade pip
pip install poetry
poetry install
```

Configuramos el kernel en vscode, para eso

- ctrl + shif + p -> reload window

Si cuando le dais a selecicionar kernel de un python env no os sugiere el que toca:

```bash
python -m ipykernel install --user --name=.faiss --display-name="FAISS"
```

- ctrl + shif + p -> reload window

Cuando ya esté seleccionado, deseactivamos el envirnoment --> deactivate

Ya estamos listos para ejecutar los notebooks
