# 🎯 Optimización de Banners con el Algoritmo del Bandido Multibrazo

**Autor:** David Licián Martínez  
**Tipo de proyecto:** Aprendizaje por Refuerzo (Reinforcement Learning) aplicado  
**Lenguaje:** Python  
**Tema:** Optimización de campañas de marketing online

---

## 🧠 Objetivo del Proyecto

Este trabajo simula una campaña de marketing digital en la que se deben optimizar banners promocionales para **maximizar el número de clics**.  
El problema se plantea como un caso clásico de **Bandido Multibrazo** (Multi-Armed Bandit), en el que hay 5 imágenes distintas que pueden ser mostradas, pero no se conoce a priori cuál es la más efectiva.

A través de un modelo de **aprendizaje por refuerzo**, se busca aprender de la experiencia (número de clics recibidos) para identificar la mejor imagen mediante la estrategia epsilon-greedy.

---

## 🔁 Enfoque técnico

Se parte de la creación de una función base que juega a los bandidos:

```python
multi_armed_bandit(num_games=1000, epsilon=0.1, verbose=False)
```

Y Sobre esta base se experimenta con distintos valores de ε (epsilon), que define el grado de exploración frente a explotación, para responder a tres preguntas clave:

1. ¿Cuál es el valor de ε que maximiza los clics?

2. ¿Cuál es la imagen que más clics obtiene y cuántos clics logró?

3. ¿Qué ocurre si se establece una ratio de explotación del 100% (ε = 0)?
