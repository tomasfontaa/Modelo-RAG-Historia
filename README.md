# Modelo RAG para Consultas sobre Historia de España - 2º Bachillerato

## 📋 Contexto

Desarrollo de un sistema de Retrieval-Augmented Generation (RAG) para responder preguntas sobre el temario de Historia de España de 2º de Bachillerato. El sistema procesa apuntes académicos, genera embeddings semánticos y permite consultas contextualizadas usando modelos de OpenAI.


## 🎯 Objetivo

Crear un asistente educativo capaz de responder preguntas específicas sobre Historia de España utilizando únicamente la información contenida en los apuntes oficiales del curso, con precisión académica y contextualización adecuada.

  
## 🛠️ Tecnologías utilizadas

Python 3.11: Lenguaje de programación principal
LlamaIndex: Framework para sistemas RAG
OpenAI GPT-3.5-turbo: Modelo generativo para respuestas
OpenAI text-embedding-3-small: Modelo de embeddings para representación semántica
PyPDF2: Procesamiento y extracción de texto desde PDF
Google Colab: Entorno de desarrollo y experimentación

## 📂 Estructura del proyecto

├── /practicaFinal_IAG.ipynb       # Notebook principal con la implementación completa
├── /apuntes.pdf                   # Documento original con los apuntes
└── /README.md                     # Este archivo

🚀 Instalación y uso

1. Instalar dependencias:
   ´´´bash
   pip install PyPDF2 llama-index llama-index-embeddings-openai
   ```
2. Configurar API key de OpenAI:
   ´´´bash
   export OPENAI_API_KEY="tu-api-key-aqui"
   ```
3. Ejecutar el notebook:
   - Abrir practicaFinal_IAG.ipynb en Google Colab o Jupyter Notebook
   - Ejecutar todas las celdas en orden
     

## 📊 Resultados

El sistema permite:

✅ Procesar automáticamente apuntes en PDF
✅ Segmentar contenido por temas mediante chunking semántico
✅ Generar embeddings vectoriales para búsqueda por similitud
✅ Responder preguntas con contexto específico y preciso
✅ Reconocer cuando no tiene información suficiente

## 👥 Autores

- Tomás Fonta
- Carlos Sainz
- Gonzalo Villar
