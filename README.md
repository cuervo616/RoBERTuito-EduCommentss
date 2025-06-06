# 🤖 Análisis de Sentimientos con RoBERTuito en Comentarios Docentes

Este repositorio implementa un modelo de análisis de sentimientos en español basado en **RoBERTuito**, una variante del modelo RoBERTa preentrenado para el idioma español, con especial enfoque en lenguaje informal y comentarios reales de estudiantes.

## Descripción General

**RoBERTuito** es un modelo _Transformer_ adaptado para tareas NLP en español. Utilizamos la versión `pysentimiento/robertuito-base-uncased` fine-tuned para clasificación de emociones y sentimientos, aplicada al análisis de comentarios estudiantiles en procesos de evaluación docente.

## Capacidades del Modelo

El modelo clasifica textos en las siguientes categorías de sentimiento:

- Positivo
- Negativo
- Neutral
- Alerta

(Se podría cambiar las etiquetas dependera del fine-tuning usado).

## Dataset de Entrenamiento

El modelo original fue entrenado con:

- Corpus de TASS (InterTASS, GeneralTASS)
- EmoEvent
- Tweets y textos en español informal

> ⚠️ Este repositorio usa modelos preentrenados y no realiza entrenamiento desde cero.

Fine-tuning

Al modelo se le realizo un ajuste fino con comentarios de estudiantes, a docentes lo cual es información privada.

> ⚠️ No se puede hacer pública esta información.

## Tecnologías Utilizadas

- `pysentimiento`
- `transformers` de Hugging Face
- `torch`
- `pandas`, `numpy`
- `scikit-learn`

### Instalación

```bash
pip install pysentimiento transformers torch
```

### Aplicación en Evaluación Docente

Este modelo se integra a un sistema de análisis de comentarios donde:

- Clasifica automáticamente los sentimientos expresados por los estudiantes.

- Genera una métrica que califica al docente según la percepción estudiantil.

Autores

- Pablo Quito - @crow616
- Juan Valdiviezo - @Gh0stJJ

Estudiantes de Ingeniería en Ciencias de la Computación

Universidad de Cuenca
