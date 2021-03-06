# Contenido del sitio

<div align="justify">

Este apartado contiene dos carpetas: [Revision1](https://github.com/mno-2020-gh-classroom/ex-modulo-3-comp-matricial-qr-dapivei/tree/master/Pruebas) y [Revision2](https://github.com/mno-2020-gh-classroom/ex-modulo-3-comp-matricial-qr-dapivei/tree/master/Pruebas/Revision2).

El folder **Revision1** contiene a su vez los siguientes documentos:

+ [prueba_precision_factorizacion_QR.ipynb](https://github.com/mno-2020-gh-classroom/ex-modulo-3-comp-matricial-qr-dapivei/blob/master/Pruebas/Revision1/prueba_precision_factorizacion_QR.ipynb): Pruebas para ver si las funciones asociadas a la factorización QR son precisas en sus cálculos, arrojan los errores correspondientes cuando la matriz es singular. Hallazgos: la función factorizacion_QR debería identificar claramente las matrices que pueden y que no pueden ser operadas. Es importante añadir una condición de validación sobre los requerimientos de la matriz de entrada cumple la siguiente condición: m >=n; en las situaciones en que el requerimiento no se cumpla, desplegar un mensaje indicando: "la matriz de entrada no es válida".

+ [pu_epbQR_sistema_sin_solucion.ipynb](https://github.com/mno-2020-gh-classroom/ex-modulo-3-comp-matricial-qr-dapivei/blob/master/Pruebas/Revision1/pu_epbQR_sistema_sin_solucion.ipynb): Pruebas para verificar si las funciones arrojan los mensajes de error correspondientes cuando la matriz de entrada no tiene las dimensiones adecuadas de entrada o cuando el sistema de ecuaciones lineales no tiene solución. Hallazgos: La función `eliminacion_bloques(A,b)` debería de ser capaz de identificar cuando se enfrenta a un sistema de ecuaciones lineales para los cuales no existe solución. En estos casos la función debería de dar como output un mensaje "Sistema de ecuaciones sin solución" o "Matriz singular" por ejemplo. Por otra parte, tambien debería validar las dimensiones de la matriz de entrada, si las dimensiones de la matriz de entrada no son cuadradas deberíamos de recibir como output un mensaje "Las dimensiones de la matriz (A) no son cuadradas, por favor revisa" por dar algun ejemplo.

+ [pu_epbQR_sistema_solucion_unica.ipynb](https://github.com/mno-2020-gh-classroom/ex-modulo-3-comp-matricial-qr-dapivei/blob/master/Pruebas/Revision1/pu_epbQR_sistema_solucion_unica.ipynb): Verificar si la función `eliminacion_bloques(A,b)` es capaz de resolver efectivamente sistemas de ecuaciones con solución única. Dados que sólo se revisaron 2 ejemplos, es necesario realizar más pruebas. Hallazgos: La función funciona perfectamente. 


+ [pu_epbQR_sistema_soluciones_infinitas.ipynb](https://github.com/mno-2020-gh-classroom/ex-modulo-3-comp-matricial-qr-dapivei/blob/master/Pruebas/Revision1/pu_epbQR_sistema_soluciones_infinitas.ipynb): Verificación de que la función `eliminacion_bloques` indica que A debe ser una matriz no singular.


El folder **Revision2** contiene a su vez los siguientes documentos:

+ [prueba2_precision_factorizacion_QR.ipynb](https://github.com/mno-2020-gh-classroom/ex-modulo-3-comp-matricial-qr-dapivei/blob/master/Pruebas/Revision2/prueba2_precision_factorizacion_QR.ipynb): Pruebas para verificar si los hallazgos identificados en el documento [prueba_precision_factorizacion_QR.ipynb](https://github.com/mno-2020-gh-classroom/ex-modulo-3-comp-matricial-qr-dapivei/blob/master/Pruebas/Revision1/prueba_precision_factorizacion_QR.ipynb) fueron atendidos. Hallazgos: 1) En esta segunda iteración de validaciones para el caso de una matriz de 5x3 (donde el número de filas es mayor al de columnas) queda confirmado que las funciones para la factorización QR se encuentran funcionando correctamente considerando los resultados obtenidos en este análisis. Al comparar numpy vs la implementación por parte de los programadores validamos que se cumple que A = QR; 2) las diferencias entre $Q$ y $R$ que también se identificaron en la primera iteración de validaciones se explican en la parte de arriba y son debidas a la "factorización thin QR" utilizada por numpy; 3) con respecto a la matriz de tamaño 3x5 (donde el número de columnas es mayor al número de filas), a la cual no es posible aplicarle la factorización QR, queda validado que el mensaje de error desplegado al correr dicha función es informativo para el usuario.

+ [pu2_epbQR_sistema_sin_solucion.ipynb](https://github.com/mno-2020-gh-classroom/ex-modulo-3-comp-matricial-qr-dapivei/blob/master/Pruebas/Revision2/pu2_epbQR_sistema_sin_solucion.ipynb): Confirmación que los issues levantados en la iteración previa de validaciones fueron atendidos satisfactoriamente por el equipo de programación. Hallazgos: La función es capaz de identificar cuando se enfrenta a un sistema de ecuaciones lineales sin solución y mandar un mensaje acorde, los mismo para el caso cuando se enfrenta a una matriz no cuadrada.

+ [pu2_epbQR_sistema_solucion_unica.ipynb](https://github.com/mno-2020-gh-classroom/ex-modulo-3-comp-matricial-qr-dapivei/blob/master/Pruebas/Revision2/pu2_epbQR_sistema_solucion_unica.ipynb): Realizar más pruebas para verificar que la función `eliminacion_bloques()`es capaz de resolver efectivamente sistemas de ecuaciones con solución única. Hallazgo: La función eliminacion_bloques(A,b) es capaz de resolver efectivamente sistemas de ecuaciones con solución única.


+ [pu2_epbQR_sistema_soluciones_infinitas.ipynb](https://github.com/mno-2020-gh-classroom/ex-modulo-3-comp-matricial-qr-dapivei/blob/master/Pruebas/Revision2/pu2_epbQR_sistema_soluciones_infinitas.ipynb): Validación de de las funciones implementadas por los programadores para resolver sistemas de ecuaciones lineales por bloques, en el módulo `funciones_factorizacion-QR`. Particularmente, busca identificar los mensajes de error emitidos por el algoritmo, cuando se enfrenta a sistemas de ecuaciones con soluciones infinitas. Hallazgos: los ejemplos muestran evidencia de que la función `eliminacion_bloques` está preparada para recibir un sistema de ecuaciones con soluciones infinitas y desplegar un mensaje de error.

</div>

