# Deep Learning Frameworks Comparison

Este repositorio contiene implementaciones de diversas arquitecturas de deep learning utilizando múltiples frameworks para comparar su rendimiento, facilidad de uso y compatibilidad.

## Objetivo

El objetivo principal de este proyecto es implementar y comparar las mismas arquitecturas de redes neuronales en diferentes frameworks de deep learning:

- **PyTorch**: Uno de los frameworks más populares con un enfoque dinámico y flexible.
- **JAX**: Framework de Google optimizado para alto rendimiento y diferenciación automática.
- **Keras**: API de alto nivel que simplifica la creación de redes neuronales (ahora como proyecto independiente, anteriormente sobre TensorFlow).

## Características

- Implementaciones paralelas de modelos clásicos y modernos en cada framework
- Comparativa de rendimiento y métricas de entrenamiento
- Exportación de modelos a ONNX para despliegue multiplataforma
- Demostraciones interactivas en Hugging Face Spaces

## Modelos Implementados

- MNIST Classifier
- [Otros modelos se añadirán próximamente]

## Exportación a ONNX

Todos los modelos serán exportados al formato ONNX (Open Neural Network Exchange), lo que permite:

- Interoperabilidad entre frameworks
- Optimización para diferentes hardware
- Despliegue en producción más eficiente
- Integración con herramientas de inferencia como ONNX Runtime

## Hugging Face Spaces

Este proyecto incluirá demostraciones interactivas utilizando [Hugging Face Spaces](https://huggingface.co/docs/hub/spaces), una plataforma que permite alojar y compartir aplicaciones de machine learning:

- **Aplicaciones interactivas**: Mediante Gradio o Streamlit
- **Demostración en tiempo real**: Visualización de las predicciones de cada modelo
- **Comparación en vivo**: Observar las diferencias entre implementaciones
- **Accesibilidad**: Las demos estarán disponibles públicamente sin necesidad de instalar nada

### ¿Qué son Hugging Face Spaces?

Hugging Face Spaces es una plataforma que permite crear, alojar y compartir demostraciones de aplicaciones de machine learning directamente en perfiles de Hugging Face. Ofrece:

- Soporte integrado para Streamlit y Gradio, facilitando la creación de interfaces de usuario
- Opciones para ejecutar en CPU o GPU según las necesidades
- Control de versiones basado en Git para colaboración
- Posibilidad de personalización mediante Docker
- Integración perfecta con modelos y datasets del ecosistema de Hugging Face

## Estructura del Proyecto

```
deep-learning/
├── pytorch/
│   └── models/
├── jax/
│   └── models/
├── keras/
│   └── models/
├── onnx_exports/
└── spaces/
    └── demo_apps/
```

## Requisitos

Se utilizará UV para la gestión de dependencias:

```bash
uv sync
uv run pytest
```

## Contribuciones

Las contribuciones son bienvenidas. Por favor, asegúrate de seguir las guías de estilo del proyecto:

- Usar type hints en todo el código Python
- Seguir la estructura de proyecto definida
- Incluir tests para las nuevas implementaciones 