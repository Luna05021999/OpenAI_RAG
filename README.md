### Proyecto OPENIARAG - Interfaz de Procesamiento de Documentos PDF con Langchain 🤖📄

Este proyecto implementa un flujo de trabajo en Python que permite cargar y procesar documentos PDF mediante técnicas avanzadas de procesamiento de lenguaje natural (NLP). Usando Langchain y OpenAI, se crea una base de datos de vectores para realizar búsquedas semánticas en documentos. Además, el proyecto incluye una interfaz interactiva construida con Gradio para que los usuarios puedan interactuar fácilmente con los documentos y obtener respuestas basadas en lenguaje natural.

📝 Descripción del Proyecto
Este proyecto está diseñado para procesar y analizar documentos PDF mediante el uso de Langchain, Chroma (como vectorstore), OpenAI para embeddings y modelos de lenguaje, y Gradio para construir una interfaz interactiva. El sistema permite:

Cargar documentos en formato PDF.
Convertir los textos en vectores para realizar consultas semánticas.
Proporcionar respuestas relevantes basadas en preguntas de los usuarios, utilizando un prompting que controla el comportamiento de la respuesta.
Probar diferentes consultas a través de una interfaz interactiva.
Características principales:
Función de respuesta: Se ha implementado una función de respuesta personalizada que procesa la consulta del usuario y devuelve la información relevante de los documentos cargados.
Chain (cadena de procesamiento): Se crea una chain que utiliza embeddings para manejar las consultas y generar respuestas contextualizadas.
ChromaDB: Almacén de vectores para realizar consultas semánticas eficientes y recuperar información.
Gradio: Interfaz de usuario amigable que permite a los usuarios interactuar con los documentos de forma sencilla.
Prompting: Un esquema de prompting para controlar el comportamiento de los modelos de lenguaje y cómo deben responder ante las consultas.

🚀 Funcionalidades
Carga y análisis de documentos PDF:

Los usuarios pueden cargar hasta 6 documentos PDF simultáneamente.
Los documentos se convierten en embeddings (representaciones vectoriales) que permiten realizar consultas semánticas precisas.
Vectorstore con Chroma:

Los embeddings de los documentos se almacenan en Chroma, lo que facilita la búsqueda rápida y eficiente de información relevante.
Función de respuesta personalizada:

Se ha desarrollado una función que procesa la consulta de los usuarios, interactúa con el vectorstore, y proporciona una respuesta en lenguaje natural basada en el contenido de los documentos.
Interfaz gráfica con Gradio:

Una interfaz fácil de usar que permite a los usuarios hacer preguntas y recibir respuestas en tiempo real, con una retroalimentación inmediata sobre los documentos cargados.
Prompting de comportamiento:

Controla el estilo y tono de las respuestas generadas por el modelo, para que sean informativas, concisas, o extensas según sea necesario.

📦 Componentes del Proyecto
1. Función de Respuesta:
Esta función toma la entrada del usuario (consulta), la envía a través de la chain, y devuelve una respuesta adecuada extraída de los documentos PDF procesados. Además, incluye un comportamiento para manejar respuestas si no se encuentra información relevante.

2. Chain de Procesamiento:
La chain se encarga de gestionar todo el flujo de trabajo desde la consulta, el vectorstore y la generación de respuestas. Integra el procesamiento de los embeddings y la consulta semántica.

3. Almacén de Vectores (ChromaDB):
Chroma almacena las representaciones vectoriales de los documentos PDF, permitiendo búsquedas rápidas y precisas de información relevante. Cada consulta realizada por el usuario se convierte en un vector, que se compara con los documentos almacenados para encontrar la respuesta más relevante.

4. Interfaz de Prueba con Gradio:
La interfaz con Gradio permite cargar documentos y realizar consultas en lenguaje natural, proporcionando una manera sencilla para que los usuarios interactúen con el sistema.

5. Prompting de Comportamiento:
Un esquema de prompting que controla cómo responde el modelo de lenguaje. Esto permite ajustar el tono de las respuestas según sea necesario, ya sea para obtener respuestas más breves o más detalladas.

🛠️ Instalación
Requisitos
Python 3.8+
OpenAI API Key (es necesaria para generar los embeddings y utilizar el modelo de lenguaje)
Instalar dependencias (ver sección de instalación)
Pasos de instalación
Clonar el repositorio: Descarga el código en tu máquina local.

Configurar el entorno virtual (opcional): Recomendamos crear un entorno virtual para gestionar las dependencias.

Instalar dependencias: Asegúrate de instalar todas las bibliotecas necesarias que están especificadas en el archivo requirements.txt.

Configurar la API de OpenAI: Asegúrate de tener una clave válida de OpenAI. Puedes crear un archivo .env o incluir tu clave directamente en la configuración del código.

Ejecutar la aplicación: Inicia el proyecto para probar la interfaz de Gradio y comenzar a hacer consultas a los documentos cargados.

📚 Tecnologías Utilizadas
Langchain: Para gestionar las cadenas de procesamiento y la integración con OpenAI.
OpenAI: Utilizado para generar embeddings y el modelo de lenguaje.
Chroma: Almacén de vectores para realizar consultas semánticas sobre los documentos cargados.
Gradio: Para crear la interfaz gráfica interactiva.
Python: Lenguaje de programación principal.

📊 Documentos Incluidos
BOE - Ley 2022
Cámara de España - Fiscalidad
Guía de Subvenciones y Ayudas
Ley 2014 Consolidada
AEPD - Gestión de Riesgos
Ciclo Vital de la Empresa

💻 Ejecución
Cargar los documentos: Los usuarios pueden cargar los documentos PDF en la interfaz de Gradio.
Realizar consultas: El sistema permite realizar preguntas en lenguaje natural y proporciona respuestas basadas en el contenido de los documentos cargados.
Visualización de respuestas: Las respuestas se muestran directamente en la interfaz, extrayendo la información más relevante de los documentos.

🤝 Contribuciones
Las contribuciones son bienvenidas. Si tienes sugerencias, preguntas o mejoras, no dudes en abrir un issue o enviar un pull request.

📋 Licencia
Este proyecto está licenciado bajo la Licencia MIT. Siéntete libre de usar y modificar el código para tus propios proyectos.

### Contacto
Luna Outerelo Fernández.
Email: lunaouterelo9@gmail.com
Linkedin: https://www.linkedin.com/in/luna-outerelo-4414a0192/