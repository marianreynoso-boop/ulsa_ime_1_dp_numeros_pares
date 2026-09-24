# Práctica 2: Guardar los números pares
## 1. Descripción del problema (Fase 1)
<!-- Explica con tus palabras qué hace tu programa y para qué serviría en la vida real. Máximo 4 líneas. -->
Mi programa identifica números pares y serviría para ayudar a sumar solo números pares en una suma que puede llegar a ser mas complicada y de esta manera se facilita el proceso
_____

## 2. Entradas y salidas (Fase 1)
<!-- Define cada entrada y cada salida, con su tipo de dato y su objetivo. -->

**Entradas:**
1. Números

**Salidas:**
1. Cuantos pares?
2. Cuales?

## 3. Restricciones e invariante (Fase 1 y 2)

**Restricciones** (¿qué debe cumplirse?):
- Deben ser 5 números
- No decimales

**Tamaño del arreglo y por qué** (piensa en el peor caso):
5 números, por si todos los números son pares

**¿El 0 y los negativos son pares? ¿Por qué?**
SI, porque siguen siendo números 

**Invariante** (¿qué es verdad después de cada vuelta del ciclo?):
Deberán de ser 5 arreglos

## 4. Casos resueltos a mano (Fase 1)

| Caso | Números | Pares guardados | Posición de cada par |
|---|---|---|---|
| 1 | 3, 8, 5, 2, 7 | 8,2 | 0,1|
| 2 | 50,10,4,7,9 | 50,10,4 | 0,1,2 |
| 3 | 6,3,45,8,13 | 6,8 | 0,1 |

## 5. Receta en pseudocódigo (Fase 2)
<!-- Tu receta va en el archivo RECETA.md. Aquí solo responde las dos preguntas. -->

**¿Probé mi receta a mano con un caso?** Sí
**¿Tuve que corregirla?** SI

## 6. Cómo compilar y ejecutar (Fase 3)

```bash
g++ -Wall -Wextra -std=c++17 main.cpp -o numeros_pares
./numeros_pares
```

## 7. Ejemplo de ejecución (Fase 3)
<!-- Pega aquí lo que muestra tu programa en pantalla con un caso normal. -->

```Guardar los numeros pares de 5 numeros
Escribe un numero: 7
Escribe un numero: 5
Escribe un numero: 6
Escribe un numero: 2
Escribe un numero: 4
Pares encontrados: 3
6 2 4 
_____
```

## 8. Experimentos (Fase 3)

**Experimento A: ¿qué apareció al imprimir las 5 posiciones del arreglo? ¿Por qué?**
Pares encontrados: 3
Porque busco los numeros pares en los arreglos

**Experimento B: ¿qué pasó al usar la variable del ciclo como posición del arreglo? ¿Por qué?**
Asignó un lugar a cada uno de los números pares, porque si fuera contador se brincaría el lugar del que no sea par

## 9. Tabla de pruebas (Fase 4)

| Caso | Números | Esperado | Obtenido | ¿Pasó? |
|---|---|---|---|---|
| Mezcla | 1, 2, 3, 4, 5 | 2 pares: 2, 4 |2 pares: 2, 4  | SI |
| Posiciones distintas | 3, 8, 5, 2, 7 | 2 pares: 8, 2 | 2 pares: 8,2 | SI |
| Todos pares | 2, 4, 6, 8, 10 | 5 pares | 5 pares | SI__ |
| Todos impares | 1, 3, 5, 7, 9 | 0 pares | 0 pares | SI_ |
| Con cero y negativos | 0, -3, -4, 7, 1 | 2 pares: 0, -4 | 2 Pares: 0, -4 | _SI |
| Entrada inválida | `hola` o `3.5` | vuelve a pedir | Entrada no valida. Escribe un numero entero. |SI|
| Caso propio 1 | -40,22,50,88,956| 5 PARES | 5 PARES| SI_ |
| Caso propio 2 |55232,654,997,-615,34 | 3 pares: 55232, 654, 34 |3 pares: 55232, 654, 34  | SI |

## 10. Bitácora de mejoras (Fase 4)

| # | ¿Qué falló o qué quise mejorar? | ¿Qué cambié? | ¿Funcionó? |
|---|---|---|---|
| 1 | Falló la receta al principio | la variable contador | _SI_ |
| 2 | ___ | _____ | _____ |

**Reto elegido (opcional):** _____

## 11. Dudas para el profesor (Fase 3)

| Duda | Lo que ya intenté |
|---|---|
| Que es una variable | Pense que era un numero diferente|

## 12. Reflexión final

**¿Qué aprendí con esta práctica?**
_____
Aprendí a escribir mejor la receta, aunque fallo un poco
**Ahora que terminé, ¿qué cambiaría de mi proceso?**
_____
Nada
**¿Qué fue lo más difícil y cómo lo resolví?**
_____
Escribir la receta, preguntado al profesor
**¿Qué pregunta me quedó sin responder?**
_____
Ninguna
**¿Por qué no puedo usar la variable del ciclo para guardar en el arreglo?**
_____
Porque el contador asigna un lugar sin importar si es par o no
## 13. Lista de verificación antes de entregar (Fase 5)

- [SI] Llené todas las secciones (no quedan `_____`)
- [SI] Mi programa compila sin advertencias
- [SI] Probé todos los casos de la tabla
- [SI] Hice los Experimentos A y B y dejé el código correcto al terminar
- [SI] No modifiqué `utilerias.h`
- [SI] Hice al menos 3 commits con mensajes claros
- [SI] Hice `git push` y verifiqué mi fork en GitHub
- [SI] Entregué el enlace de mi fork en Classroom