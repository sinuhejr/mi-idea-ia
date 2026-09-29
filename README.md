# GastoClaro: clasificador de gastos con IA

Final project for the Building AI course

## Summary
Una app que lee la descripción de tus gastos (por ejemplo, "Uber a la escuela" o "tacos con amigos") y los clasifica sola en categorías como transporte, comida o entretenimiento, para que veas en qué se va tu dinero sin capturar nada a mano.

## Antecedentes
Mucha gente quiere llevar control de sus gastos, pero abandona la costumbre porque clasificar cada compra es tedioso. Resolver esto ayuda a tener mejores hábitos financieros, sobre todo a estudiantes y jóvenes que empiezan a manejar su dinero.

## Cómo se usa
1. Subes el estado de cuenta de tu banco o escribes tus gastos.
2. La IA asigna una categoría a cada uno.
3. Ves un resumen mensual con gráficas y alertas, por ejemplo: "Este mes gastaste 30% más en comida".

## Datos y métodos de IA
- **Datos:** descripciones de gastos ya etiquetadas con su categoría (al inicio, unos cientos de ejemplos).
- **Método:** clasificación de texto con una bolsa de palabras (bag of words) y un clasificador Naive Bayes, como vimos en el curso. Más adelante se podría mejorar con una red neuronal.
- **Aprendizaje:** si el usuario corrige una categoría, el modelo aprende de esa corrección.

## Desafíos
- **Privacidad:** los datos financieros son sensibles, así que se procesarían solo en el dispositivo del usuario.
- **Errores:** descripciones ambiguas como "OXXO" pueden ser comida, transporte o hogar.
- **Sesgo:** el modelo aprende de los hábitos de quien lo entrena y puede fallar con otros estilos de vida.

## Qué sigue
- Predecir el gasto del próximo mes con regresión.
- Recomendar metas de ahorro personalizadas.

## Agradecimientos
Proyecto inspirado en el curso Elements of AI de la Universidad de Helsinki y Reaktor.
