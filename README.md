![](https://github.com/arigarmendia/NLP/blob/main/banner_NLP.png)

##  Ariadna Garmendia - Carrera de Especialización en Inteligencia Artificial  <br /><br />

> ###   Contenido: <br />

*   ⭐ Desafío 1: [Word2vec](https://github.com/arigarmendia/NLP/blob/main/Desafio_1/Word2vector.ipynb)<br />
    Implementación de varias funciones para transformar palabras a vectores, utilizando únicamente Numpy. Incluye identificación del vocabulario del corpus, transformación de los documentos del corpus con One-Hot encoding, TF, TF-IDF y una función para calcular Similitud Coseno.  

*   ⭐ Desafío 2: [Bot](https://github.com/arigarmendia/NLP/blob/main/Desafio_2/bot.ipynb) <br />
    Implementación de un Bot simple en Español con librería Spacy Stanza. El bot busca la respuesta por medio del cálculo de Similitud coseno comparando con todas las frases de un corpus previamente transformadas con TF-IDF. El texto del corpus fue tomado de una página Web que contiene frases icónicas de los Simpsons. 

*   ⭐ Desafío 3: [Custom embeddings con Gensim](https://github.com/arigarmendia/NLP/tree/main/Desafio_3) <br />
    Generación y ensayo de embeddings creados con la librería Gensim a partir de los modelos CBOW y Skipgram. Los embeddings se generaron a partir de un corpus en español basado en el cuento "El caballero de la armadura oxidada". Para visualizar agrupación entre vectores se utilizó TSNE con librería Sklearn.

*   ⭐ Desafío 4: [Predictor de próxima palabra](https://github.com/arigarmendia/NLP/blob/main/Desafio_4/pred_next_word.ipynb) <br />
    Ensayo de predictor "many-to-one" utilizando embeddings y redes LSTM. Se utilizó un corpus basado en letras de canciones en inglés de la banda Coldplay (aprox. 62k palabras). Adicionalmente se probó un generador de secuencias autorregresivo utilizando los modelos ensayados.

*   ⭐ Desafío 5: [Sentiment analysis](https://github.com/arigarmendia/NLP/tree/main/Desafio_5)<br />
    Sentiment analysis utilizando el [dataset](https://www.kaggle.com/datasets/nicapotato/womens-ecommerce-clothing-reviews/code) de ecommerce clothing reviews de Kaggle. Se utilizaron custom embeddings y embedding pre-entrenados Fasttext con arquitectura de redes LSTM bidireccionales y se ejecutaron pruebas con y sin stop-words. Se implementaron técnicas de undersampling y entrenamiento con pesos (class_weights) para contrarrestar los efectos del desbalance de clases en el dataset.


*   ⭐ Desafío 6: [bot_qa](https://github.com/arigarmendia/NLP/tree/main/Desafio_6)<br />
    Bot de preguntas y respuestas, conformado a partir de una arquitectura encoder-decoder con embeddings pre-entrenados Fasttext. Se analizaron 3 modelos basados en esencialmente la misma arquitectura pero con algunas variaciones (agregado de distintas opciones de dropout para mitigar el overfitting). <br /><br />

![](https://github.com/arigarmendia/NLP/blob/main/herramientas.png)<br /><br />

> ### 💡 Estructura del repositorio:<br />
```bash
├── Desafio_1
│   ├── Word2vector.ipynb
├── Desafio_2
│   ├── bot.ipynb
├── Desafio_3
│   ├── my_embeddings.ipynb
│   ├── graficos_TSNE
├── Desafio_4
│   ├── pred_next_word.ipynb
│   ├── dataset
├── Desafio_5
│   ├── Desafio5_Notebook1.ipynb
│   ├── Desafio5_Notebook2.ipynb
│   ├── Pruebas_extra.ipynb
│   ├── dataset
│       ├── clothing_ecommerce_reviews.csv
├── Desafio_6
│   ├── bot_qa_model1.ipynb
│   ├── bot_qa_model2.ipynb
│   ├── bot_qa_model3.ipynb
│   ├── conclusiones.md
├── README.md
├──.gitignore
```
<br />

####    Preguntas? ✉️ arigarmendia@gmail.com