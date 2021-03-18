# kedro
tutorial kedro


## Instalación de kedro 
### Preparar entorno e instalación 

Crear un entorno virtual 

```cmd
py -m venv env/kedro-environment
```

Activar el entorno 

```cmd
source env/kedro-environment/Scripts/activate
```

Instalación 

```cmd
pip install kedro 
```

### Preparar entorno e instalación (anaconda)


Crear un entorno virtual 

```cmd
conda create --name kedro-environment python=3.7 -y 
```

Activar el entorno 

```cmd
conda activate kedro-environment
```

Instalación 

```cmd
pip install kedro 
```
## Tipico Workflow con kedro 


```cmd
kedro new --starter=spaceflights 
```

paso que se van a seguir 
1. set up project template
2. set up data 
3. create a pipeline
4. package the project 


1. Set up the project template
Create a new project with kedro new

Install project dependencies with kedro install

Configure the following in the conf folder:

Logging

Credentials

Any other sensitive / personal content

2. Set up the data
Add data to the data/ folder

Reference all datasets for the project in conf/base/catalog.yml

3. Create the pipeline
Create the data transformation steps as Python functions

Construct the pipeline by adding your functions as nodes

Choose how to run the pipeline: sequentially or in parallel

4. Package the project
Build the project documentation

Package the project for distribution
