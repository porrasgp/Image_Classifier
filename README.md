# Diagrama de Flujo - Aplicación de Puntos GPS y Machine Learning

```flow
st=>start: Inicio
e=>end: Fin
op1=>operation: Tomar foto y GPS diariamente
op2=>operation: Guardar en Base de Datos
op3=>operation: Consultar Base de Datos
op4=>operation: Aplicar Algoritmo de Machine Learning
op5=>operation: Limpiar las Imágenes
op6=>operation: Realizar Sugerencias
cond=>condition: ¿Sugerencias listas?

st->op1->op2->op3->op4->op5->op6->cond
cond(yes)->e
cond(no)->op6
