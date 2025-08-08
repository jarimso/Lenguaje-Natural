# Universidad Icesi - Curso de Natural Language Processing (NLP)

Repositorio para material de apoyo al curso de NLP en Universidad Icesi, Cali, Colombia.

## Tabla de Contenidos

- [Estructura del repositorio](#estructura-del-repositorio)
- [Configuración del Entorno](#configuración-del-entorno)
  - [Opción 1: Usando UV (Recomendado)](#opción-1-usando-uv-recomendado)
  - [Opción 2: Usando pip y requirements.txt](#opción-2-usando-pip-y-requirementstxt)
  - [Opción 3: Usando Conda](#opción-3-usando-conda)
- [Sesiones](#sesiones)
  - [Sesión 1 - NLP Clásico](#sesión-1---nlp-clásico)
  - [Sesión 2 - Word Embeddings](#sesión-2---word-embeddings)
  - [Sesión 3 - Transformers](#sesión-3---transformers)
  - [Sesión 4 - BERT y Finetunning](#sesión-4---bert-y-finetunning)
  - [Sesión 5 - Generación de texto](#sesión-5---generación-de-texto)
  - [Sesión 6 - Retrieval Augmented Generation](#sesión-6---retrieval-augmented-generation)

### Estructura del repositorio

```bash
├── .gitignore
├── .python-version
├── .venv/
├── environment.yaml
├── LICENSE
├── pyproject.toml
├── README.md
├── requirements.txt
├── uv.lock
├── Sesion1
│   ├── 1-spacy-basics.ipynb
│   ├── 2-tokenization.ipynb
│   ├── 3-stemming.ipynb
│   ├── 4-lemmatization.ipynb
│   ├── 5-vocabulary.ipynb
│   ├── 6-practice.ipynb
│   ├── 7-sentiment-analysis.ipynb
│   ├── covid-19_vaccine_tweets_with_sentiment.csv
│   ├── JFKIA.txt
│   ├── moviereviews.tsv
│   ├── owlcreek.txt
│   └── reaganomics.txt
├── Sesion2
│   └── 1-semantics-word-vectors.ipynb
├── Sesion3
│   └── 1-transformers-from-scratch.ipynb
├── Sesion4
│   └── 1-text-classification-with-hf.ipynb
├── Sesion5
│   └── 1-text-generation.ipynb
└── Sesion6
    └── 1-ollama-rag.ipynb
```

Este repositorio esta diseñado para servir como referencia funcional de las lecciones del curso. Cada sesión del curso tiene su propio directorio con notebooks de Jupyter con el material técnico visto en las lecciones y de donde el estudiante se puede valer para hacer sus propios entregables.

Los notebooks pueden ser ejecutados en Google Colab de forma individual y auto-suficiente. Además, se ofrecen los respectivos environment.yaml y requirements.txt para crear en local via Anaconda o virtualenv un entorno de trabajo de python donde puedan ser ejecutados los ejercicios en forma local.

## Configuración del Entorno

### Opción 1: Usando UV (Recomendado)

[UV](https://docs.astral.sh/uv/) es un administrador de paquetes de Python ultra-rápido. Para configurar el entorno:

1. **Instalar UV** (si no lo tienes instalado):

   ```bash
   # En Windows
   powershell -c "irm https://astral.sh/uv/install.ps1 | iex"
   
   # En macOS/Linux
   curl -LsSf https://astral.sh/uv/install.sh | sh
   ```

2. **Instalar dependencias**:

   ```bash
   uv sync
   ```

### Opción 2: Usando pip y requirements.txt

Si prefieres usar pip tradicional:

1. **Crear entorno virtual**:

   ```bash
   python -m venv .venv
   
   # En Windows
   .venv\Scripts\activate
   
   # En macOS/Linux
   source .venv/bin/activate
   ```

2. **Instalar dependencias**:

   ```bash
   pip install -r requirements.txt
   ```

### Opción 3: Usando Conda

Para usuarios de Anaconda o Miniconda:

```bash
conda env create -f environment.yaml
conda activate icesi-nlp
```

## Sesiones

### Sesión 1 - NLP Clásico

- [NLP Básico con SpaCy](./Sesion1/1-spacy-basics.ipynb)
- [Tokenización](./Sesion1/2-tokenization.ipynb)
- [Stemming](./Sesion1/3-stemming.ipynb)
- [Lemmatization](./Sesion1/4-lemmatization.ipynb)
- [Vocabularios](./Sesion1/5-vocabulary.ipynb)
- [Práctica](./Sesion1/6-practice.ipynb)
- [Análisis de Sentimientos](./Sesion1/7-sentiment-analysis.ipynb)

### Sesión 2 - Word Embeddings

- [Semantica y vectores de palarba](./Sesion2/1-semantics-word-vectors.ipynb)

### Sesión 3 - Transformers

- [Transformers desde cero](./Sesion3/1-transformers-from-scratch.ipynb)

### Sesión 4 - BERT y Finetunning

- [Clasificación de texto con Hugging Face](./Sesion4/1-text-classification-with-hf.ipynb)

### Sesión 5 - Generación de texto

- [Generación de texto con modelos GPT](./Sesion5/1-text-generation.ipynb)

### Sesión 6 - Retrieval Augmented Generation

- [Ollama RAG](./Sesion6/1-ollama-rag.ipynb)
