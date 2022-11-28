![Tec de Monterrey](images/logotecmty.png)
# Act 5.2 - Actividad Integral sobre el uso de códigos hash (Evidencia Competencia)

## <span style="color: rgb(26, 99, 169);">¿Qué tengo que hacer?</span>
En este repositorio encontrarás los archivos de entrada, así como las salidas esperadas que podrás usar para probar tu implementación. También encontrarás un archivo "main.cpp". Ahí deberás implementar tu solución. En el archivo deberás colocar en la parte superior, en comentarios, tus datos. Por ejemplo:
```
// =========================================================
// File: main.cpp
// Author: Edward Elric - A00123456
// Date: 01/01/2021
// =========================================================
```
<span style="text-decoration: underline;">De manera individual</span>, desarrolla la solución del siguiente problema:

Como en cualquier empresa, en la compañía naviera "International Seas, LTD." cada empleado tiene una descripción de su puesto de trabajo. Una descripción contiene unos pocos párrafos que describe las responsabilidad del puesto. Esta, junto con otros factores, como la antigüedad, se utiliza para determinar su salario.

En la empresa hemos desarrollado el sistema "Unlimited Seas". Este sistema libera al departamento de Recursos Humanos de tener que hacer un juicio inteligente sobre el valor del empleado; la descripción del puesto simplemente se escanea en busca de palabras y frases que indiquen responsabilidad. En particular, las descripciones de puestos que indican el control de un gran presupuesto o la gestión de un gran número de personas producen puntuaciones alta en "Unlimited Seas".

Lo que haremos en este activad, será implementar un sistema "Unlimited Seas" simplificado. Recibirás como entrada un diccionario y una serie de descripciones de puestos. Para cada descripción, deberás calcular el salario asociado con el puerto, de acuerdo con el sistema.

## <span style="color: rgb(26, 99, 169);">**Entrada**</span>
La primera línea de entrada contiene 2 números enteros positivos: *m* ≤ 1,000, el número de palabras en diccionario "Unlimited Seas", y *n* ≤ 100, el número de descripciones de puestos. Las siguientes *m* líneas; cada una contiene una palabra y un valor en dólares (un número entero entre 0 y 1,000,000). A continuación, se encuentran las n descripciones de puestos. Cada descripción de puesto de trabajo consta de uno o más líneas de texto; para mayor facilidad, el texto se ha convertido a minúsculas y no tiene más caracteres que letras, números y espacios. Cada descripción de puesto de trabajo con una línea que contiene un punto.

## <span style="color: rgb(26, 99, 169);">**Salida**</span>
Para cada descripción de puesto de trabajo, deberás calcular el salario correspondiente calculado como la suma de los valores de "Unlimited Seas" para todas las palabras que aparecen en la descripción. Las palabras que no aparecen en el diccionario tienen un valor de 0. A continuación encontrarás un ejemplo de entrada y salida.

## <span style="color: rgb(26, 99, 169);">**Ejemplo de entrada**</span>
7 2 <br>
administer 100000 <br>
spending 200000 <br>
manage 50000 <br>
responsibility 25000 <br>
expertise 100 <br>
skill 50 <br>
money 75000 <br>
the incumbent will administer the spending of kindergarden milk money
and exercise responsibility for making change he or she will share
responsibility for the task of managing the money with the assistant
whose skill and expertise shall ensure the successful spending exercise <br>
. <br>
this individual must have the skill to perform a heart transplant and
expertise in rocket science <br>
. <br>

## <span style="color: rgb(26, 99, 169);">**Ejemplo de salida**</span>
700150 <br>
150 <br>

Para probar tu implementación, compila tu programa con el comando:
```
g++ -std=c++11 main.cpp -o app
```
Posteriormente, prueba con cada uno de los archivos de entrada de prueba que encontrarás en este repositorio (input1.txt, input2.txt, input3.txt, input4.txt). Los resultados que debes obtener se encuentran en los archivos llamados output1.txt, output1.txt, output1.txt y output1.txt. Para realizar las pruebas, puedes usar las siguientes líneas de código. Por ejemplo, si queremos probar con el archivo de prueba "input1.txt".
```
./app < input1.txt > mysolution1.txt
diff mysolution1.txt output1.txt
```
Si el segundo comando no tenga ninguna salida, sabrás que los resultados que obtuviste son los esperados. Recuerda actualizar tu repositorio (*git push*) cuando hayas terminado tu implementación.

Por último, realiza una investigación y reflexión de la importancia y eficiencia del uso de las tablas hash para tales fines,  generando un documento llamado **"ReflexAct5.2.pdf"**

## <span style="color: rgb(26, 99, 169);">**¿Bajo qué criterios se evalúa mi evidencia?**</span>

- **80%** - Para cada una de las funcionalidades se evaluará:

    - **Excelente (80%)** - pasa correctamente todos los casos de prueba.
    - **Muy Bien (60%)** - pasa correctamente el 75% de los casos de prueba.
    - **Bien (40%)** - pasa correctamente el 50% de los casos de prueba.
    - **Insuficiente (20%)** - pasa correctamente menos del 50% de los casos de prueba.


- **10%** - El código deberá seguir los lineamientos estipulados en el estándar de codificación: <span class="instructure_file_holder link_holder">[liga_estándar_codificación](estandar.pdf)</span>
- **10%** - Se respetenan los nombres de las funciones en la aplicación.

## <span style="color: rgb(26, 99, 169);">**¿Dónde la entrego?**</span>
Esta actividad forma parte tanto de tu calificación final del curso, así como del portafolio de evidencias de las competencias a desarrollar del curso, por lo que se te pide que en forma individual:
* Realices una entrega del código fuente de la solución del problema, en la sección correspondiente dentro de esta plataforma, así como el documento de reflexión individual (**ReflexAct5.2.pdf**).
En la carpeta personal llamada **TC1031(Portafolio_Final)** que generaste desde la entrega de la actividad 1.3 y que te servirá como preparación para la entrega del portafolio de competencias que se realizará al final del curso, coloca en la subcarpeta **Act5.2** tus archivos que solucionaron la <span style="text-decoration: underline;">actividad 5.2</span> así como el documento de reflexión individual (**ReflexAct5.2.pdf**).
