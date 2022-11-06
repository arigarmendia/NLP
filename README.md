# NLP
Repositorio para la materia Procesamiento del Lenguaje Natural

Estructura del repositorio:
```bash
├── Desafio_1
│   ├── Word2vector.ipynb
├── Desafio_2
│   ├── bot.ipynb
├── README.md
├──.gitignore
```
Descripción de los trabajos:
*   Desafío 1: Word2vec
    Implementación de varias funciones para transformar palabras a vectores, utilizando únicamente Numpy. Incluye identificación del vocabulario del corpus, transformación de los documentos del corpus con One-Hot encoding, TF, TF-IDF y una función para calcular Similitud Coseno.  

*   Desafío 2: Bot 
    Implementación de un Bot simple en Español con librería Spacy Stanza. El bot busca la respuesta por medio del cálculo de Similitud coseno comparando con todas las frases de un corpus previamente transformadas con TF-IDF. El texto del corpus fue tomado de una página Web que contiene frases icónicas de los Simpsons. 