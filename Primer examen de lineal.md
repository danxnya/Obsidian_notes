
1.  <mark style="background: #D2B3FFA6;">Eliminacion de Gauss Jordan</mark>

Lo único que se necesita hacer es poner nuestras ecuaciones en forma de matriz para poder<span style="color:#e37ff0"> transformarlas</span> en la matriz **identidad**. hecho esto obtendremos los valores con los cuales se resuelve la matriz.
![[WhatsApp Image 2023-09-28 at 9.05.03 PM.jpeg|460]]

2. <mark style="background: #D2B3FFA6;">Operaciones aritmeticas entre matrices</mark>
 
- Cuando vamos a multiplicar un escalar; ya sea definido o no, solo necesitamos multiplicarlo por cada una de los valores de nuestra matriz.
- En la suma/resta solo y solo si las dos matrices son del <span style="color:#e37ff0">mismo tamaño</span> se podrá efectuar la suma.
- Para multiplicar dos matrices es muy importante revisar las dimensiones. Cuando hacemos la multiplicación, la matriz 1 debe multiplicar sus filas por las columnas de la matriz 2. En caso de que no alcancen los valores no tendrá solución esa operación.  
![[WhatsApp Image 2023-09-28 at 9.27.43 PM.jpeg|480]]

3. <mark style="background: #D2B3FFA6;">Inversa por Gauss Jordan</mark>

Para calcular la inversa con el método GJ habrá que crear una matriz identidad a la derecha de la matriz original, de tal forma que la matriz original con operaciones aritméticas se convierta en la identidad, de esta forma en donde estaba la identidad obtendremos la inversa de nuestra matriz. (<span style="color:#00b0f0">Solo usar este metodo si no se admite por Adjunta</span>)

4. <mark style="background: #D2B3FFA6;">Determinante</mark>

Hay varios métodos para calcular el determinantes pero el más eficaz es <span style="color:#e37ff0">cofactores</span> que consiste en tapar la fila o columna que tenga más ceros para simplificarlo lo más posible, recorrer la fila/columna respetando los <span style="color:#e37ff0">signos</span> de la matriz (+, -) y multiplicar de forma cruzada la parte que no es tapada en filas ni columnas para posteriormente sumarlos.
![[WhatsApp Image 2023-09-28 at 9.47.17 PM.jpeg|490]]

5. <mark style="background: #D2B3FFA6;">Cramer</mark>

Para usar el método de cramer para encontrar la solución a un sistema de ecuaciones primero que nada se debe calcular el determinante (<span style="color:#00b0f0">En caso de que este de 0, hay soluciones infinitas o no hay ninguna</span>)  sabiendo el valor de "det(**Δ**)", lo que toca hacer es crear la matriz de las variables y usar las constantes de los resultados como coeficiente x,y,z según sea el caso. Con esto solo tendremos que seguir la formula de:
$\mathbb{Sol =} \frac{Δx}{Δ}, \space \frac{Δy}{Δ}, \space \frac{Δz}{Δ}$
![[WhatsApp Image 2023-09-28 at 8.05.30 PM.jpeg|478]]

6. <mark style="background: #D2B3FFA6;">Inversa con la adjunta</mark>

- El primer paso será calcular Δ (Escalar)
- Después la adjunta (Matricial), esta se calcula seleccionando la fila/columna con más ceros de la misma forma que el Δ, con la diferencia de que no se toman en cuenta los valores que se han tapado seleccionando su fila y columna, ademas de respetarse los signos(+, -).
Cuando tenemos Δ y la Adjunta solo necesitamos usar una formula que dice:
$\mathbb{Sol = } \frac{1}{Δ} * |Adj|$ 
![[WhatsApp Image 2023-09-28 at 9.47.15 PM.jpeg|470]]
