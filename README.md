Generación de Base de Datos con Estimadores Predeterminados Aquí no se extraen muestras: se diseñan universos con intención.
📌 Propósito Este script crea una base de datos sintética donde el usuario define los parámetros poblacionales del modelo lineal simple (α, β) y las propiedades estadísticas de las variables involucradas. El resultado es una muestra calibrada, ideal para estimaciones limpias, pruebas didácticas o simulaciones posteriores.
⚙️ Parámetros configurables | Parámetro | Descripción | Valor por defecto | | N | Tamaño muestral | 100 | | μₓ (mu_x) | Media de la variable x | 20 | | σₓ (sigma_x) | Desvío estándar de x | 15 | | α (alpha) | Término constante del modelo | 5 | | β (beta) | Coeficiente de x | 2 | | σₑ (sigma_e) | Desvío del error aleatorio | 10 |
🧠 Metodología
- Se genera x a partir de una distribución normal estándar, ajustada para tener media μₓ y desviación σₓ exactas.
- Se genera u (error) con media cero y desviación σₑ, también con ajuste exacto.
