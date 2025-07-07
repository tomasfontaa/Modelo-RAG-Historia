# Modelo RAG para Consultas sobre Historia de España

Este proyecto implementa un sistema RAG (Retrieval-Augmented Generation) para responder preguntas sobre Historia de España utilizando documentos académicos como fuente de información.

## Descripción

El sistema procesa un PDF con apuntes de Historia de España (2º de Bachillerato) y permite realizar consultas específicas sobre los temas contenidos en el documento, proporcionando respuestas precisas basadas en el contenido original.

## Características principales

- Segmentación semántica automática: Divide el documento PDF en 18 temas históricos distintos.
- Generación de embeddings: Utiliza el modelo text-embedding-3-small de OpenAI para crear representaciones vectoriales del contenido.
- Búsqueda semántica: Recupera información relevante basada en el significado de la consulta.
- Respuestas contextuales: Genera respuestas utilizando el modelo gpt-3.5-turbo de OpenAI, limitándose estrictamente al contenido de los documentos.

## Estructura del proyecto

/practicaFinal_IAG.ipynb       Notebook principal con la implementación completa
/temas_historia/               Contiene los temas segmentados en archivos TXT
/historia_index/               Almacena el índice vectorial para búsquedas rápidas

## Requisitos

Para ejecutar este proyecto necesitarás:

- Python
- Las siguientes librerías Python:
  - PyPDF2
  - llama-index
  - llama-index-embeddings-openai
    
- Una API key de OpenAI (configurada como variable de entorno OPENAI_API_KEY)

## Uso

1. Carga el documento PDF original (apuntes.pdf)
2. El notebook procesará automáticamente el contenido, dividiéndolo en temas
3. Genera los embeddings y construye el índice vectorial
4. Realiza consultas como:
  - "¿Qué consecuencias tuvo el Sexenio Revolucionario?"
  - "Dime un resumen de la dictadura de Francisco Franco"

El sistema está configurado para responder únicamente basándose en el contenido de los documentos, evitando especulaciones o información externa.
