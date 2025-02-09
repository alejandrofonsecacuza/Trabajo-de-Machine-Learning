
# Chest X-Ray Image Classification using MobileNetV2


## Descripción del Proyecto

El proyecto utiliza un conjunto de datos de imágenes de rayos X de tórax para entrenar un modelo de Deep Learning basado en MobileNetV2, una red neuronal convolucional eficiente y ligera. El modelo se entrena para clasificar las imágenes en las categorías correspondientes.

### Conjunto de Datos

El conjunto de datos utilizado en este proyecto es [Chest X-Ray Images (Pneumonia)](https://www.kaggle.com/paultimothymooney/chest-xray-pneumonia), que contiene imágenes de rayos X de tórax etiquetadas. 

### Requisitos

Para ejecutar este proyecto, necesitas tener instalado lo siguiente:

- Python 3.8 o superior
- TensorFlow 2.x
- Keras
- OpenCV
- Matplotlib
- NumPy
- Pandas

Puedes instalar las dependencias ejecutando:

```bash
pip install -r requirements.txt
```

### Estructura del Proyecto

```
chest-xray-classification/
├── app/                     # Código fuente del proyecto
│   ├── Visualizacion.ipynb
│   ├── Descargar Dataset.ipynb
│   ├── Creacion dataset y preprocesamiento.ipynb      
│   ├── Entrenamiento.ipynb  
│   └── Resultados.ipynb
├── requirements.txt         # Dependencias del proyecto
├── Dockerfile               # Dockerfile para construir la imagen del proyecto
└── README.md                # Este archivo
```



### Uso del Modelo


#### Clonar el Repositorio

Primero, clona el repositorio en tu máquina local:

```bash
git clone https://github.com/alejandrofonsecacuza/Trabajo-de-Machine-Learning.git
cd Trabajo-de-Machine-Learning
```

### Usar Docker

Puedes construir y ejecutar este proyecto usando Docker para evitar problemas de compatibilidad con dependencias.

#### Construir la Imagen de Docker

1. Asegúrate de tener Docker instalado en tu sistema.
2. Navega a la raíz del proyecto donde se encuentra el `Dockerfile`.
3. Construye la imagen de Docker ejecutando:

```bash
docker build -t chest-xray-classification .
```

#### Ejecutar el Contenedor

Una vez que la imagen esté construida, puedes ejecutar el contenedor con:

```bash
docker run -p 8888:8888 chest-xray-classification
```

Esto iniciará Jupyter Notebook dentro del contenedor y lo expondrá en el puerto 8888 de tu máquina local. Abre tu navegador y visita `http://localhost:8888` para acceder a Jupyter Notebook.


### Contribuciones

Las contribuciones son bienvenidas. Si deseas mejorar este proyecto, por favor abre un issue o envía un pull request.

### Licencia

Este proyecto está bajo la licencia [MIT](LICENSE).

