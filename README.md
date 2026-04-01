[![Open in MATLAB Online](https://www.mathworks.com/images/responsive/global/open-in-matlab-online.svg)](https://matlab.mathworks.com/open/github/v1?repo=Adriana-03-b/MSFPractica3)

# Práctica 3: Sistema Musculoesqueletico

## Información de la estudiante

Bañuelos Adriana \[23210694]; L23210694@tectijuana.edu.mx

Modelado de Sistemas Fisiológicos

Ingeniería Biomédica

## Docente

Dr. Paul Antonio Valle Trujillo; paul.valle@tectijuana.edu.mx

Departamento de Ingeniería Eléctrica y Electrónica, Tecnológico Nacional de México/IT Tijuana, Blvd. Alberto Limón Padilla s/n, Tijuana, C.P. 22454, B.C., México.

## Descripción de la asignatura

El modelizado de sistemas fisiológicos es una herramienta importante en Ingeniería Biomédica, permite comprender el funcionamiento del cuerpo humano, así como diseñar y evaluar terapias y dispositivos médicos; se define como el proceso de formular modelos matemáticos o computacionales que representan el comportamiento y la interacción de los sistemas biológicos y fisiológicos. Esta asignatura pretende aportar al perfil del Ingeniero Biomédico la capacidad de realizar investigación científica en el área de Biología de Sistemas con la finalidad de dirigir y participar en equipos de trabajo interdisciplinarios en contextos nacionales e internacionales, así como de proporcionar soluciones informáticas para resolver problemas en el campo de la Ingeniería Biomédica con ética profesional; lo anterior al proporcionar al estudiante bases sólidas para modelizar sistemas y diseñar controladores para la solución de problemas en las áreas de atención médica y del sector industrial médico. La construcción de analogías entre circuitos eléctricos y sistemas fisiológicos para la formulación de modelos matemáticos y el diseño de controladores mediante la experimentación in silico brindan herramientas de gran aplicación en el quehacer profesional del Ingeniero Biomédico.

La asignatura de Modelado de Sistemas Fisiológicos forma parte del plan de estudios de la carrera en Ingeniería Biomédica con la siguiente competencia general del curso: Utiliza las propiedades de los circuitos RLC para describir la dinámica de sistemas fisiológicos, obtener modelos matemáticos y aplicar el control clásico, esto con el objetivo de integrar los principios de la Ingeniería de Control, la Electrónica Analógica y las Ciencias de la Computación con la Anatomía y Fisiología del cuerpo humano para proporcionar descripciones cuantitativas y cualitativas de sistemas fisiológicos complejos con el objetivo de modelizar, analizar, controlar, ilustrar y predecir su dinámica tanto en el corto como en el largo plazo.

## Objetivos

1\. Calcular la función de transferencia.
2. Determinar el modelo de ecuaciones integro-diferenciales.
3.Modelar el sistema musculoesquelético utilizando un sistema masa-resorte-amortiguador equivalente que represente sus propiedades fisiológicas.
4.Identificar la función del elemento contráctil activo (actina-miosina) en la generación de fuerza muscular.
5.Evaluar el comportamiento de los elementos elásticos:
En paralelo 𝐶𝑝, asociado al tejido conectivo.
En serie 𝐶𝑠, relacionado con los tendones.
6.Simular el modelo en un entorno computacional (por ejemplo, Simulink) para observar la respuesta del sistema ante diferentes condiciones de entrada.
Interpretar los resultados obtenidos en la simulación desde un punto de vista fisiológico.
7. Obtener la respuesta en lazo abierto y en lazo cerrado con el controlador PI en Spyder/Python con la función de transferencia.

## Descripción detallada del sistema
Michael Khoo modeliza un compartimento del sistema musculoesquelético mediante el diagrama mecánico.
El modelo musculoesquelético presentado corresponde a un sistema mecánico equivalente que incluye elementos activos y pasivos para describir el comportamiento del músculo. Debido a la presencia de un elemento elástico en paralelo y una combinación en serie de elementos viscoelásticos, el sistema requiere al menos dos variables de estado para representar su dinámica. El vector de estados puede definirse mediante las variables x(t), que representa el desplazamiento total del sistema, y x1(t) que corresponde a la elongación del elemento elástico en serie.
En este modelo, F(t) representa la fuerza total aplicada al sistema, mientras que F0 es la fuerza generada por el elemento contráctil activo del músculo, cumpliendo la relación 0<α<1. Los parámetros del sistema incluyen R, que modela la amortiguación viscosa del tejido muscular Cp; , que representa la elasticidad en paralelo asociada al sarcolema; y Cs , que corresponde a la elasticidad en serie vinculada a los tendones.
La configuración en paralelo implica que el desplazamiento total x(t) es compartido entre las ramas del sistema, mientras que en la rama en serie, la suma de las deformaciones del amortiguador 𝑅 y el resorte Cs ​es igual a x(t). Sin embargo, cada elemento puede deformarse de manera diferente, por lo que se introduce x1(t)como la deformación del resorte en serie, resultando que la deformación del amortiguador es x(t)-x1(t).

Este modelo presenta varias ventajas importantes, por ejemplo:

1.Permite representar de manera sencilla la interacción entre los componentes activos y pasivos del músculo mediante pocos elementos mecánicos.
2.Existe una analogía directa entre los elementos mecánicos (resortes y amortiguadores) y las propiedades fisiológicas del tejido muscular, facilitando la interpretación biomecánica del sistema.
3.Es útil para analizar la respuesta dinámica del músculo ante diferentes estímulos de fuerza, considerando tanto efectos elásticos como viscosos.
Palabras clave: Sistema musculoesquéletico; Análisis matemático; ; Modelo de Michel Khoo; Función de transferencia; Superposición.

## Lista de archivos incluidos en el repositorio

1\. Cuaderno computacional de MATLAB \[.mlx].
2. Modelo de Simulink \[.slx].
3. Archivos de Spyder \[.py].
4. Imagen con los parámetros del controlador.
5. Imágenes de las simulaciones \[.pdf].
6. Evidencia del análisis matemático: función de transferencia, modelo de ecuaciones integro-diferenciales, error en estado estacionario y estabilidad en lazo abierto.

7\. Modelo fisiológico en Biorender o BioArt.

## Referencias

\[1] P. A. Valle, Syllabus para Modelado de Sistemas Fisiológicos, Tecnológico Nacional de México / Instituto Tecnológico de Tijuana, Tijuana, B.C., México, 2025. Permalink: https://biomath.xyz/course/

\[2] M. C. Khoo, Physiological Control Systems Analysis Simulation, and Estimation, 2nd ed. Piscataway, New Jersey, USA: IEEE Press, 2018, Section 4, Page 93.

\[3] N. S. Nise, Control Systems Engineering, 8th ed. Hoboken, New Jersey, USA: John Wiley \& Sons, 2020.

\[4] T. Kind, T. J. Faes, J. W. Lankhaar, A. Vonk-Noordegraaf \& M. Verhaegen, "Estimation of three-and four-element Windkessel parameters using subspace model identification", IEEE Transactions on Biomedical Engineering, vol. 57, issue 7, pp. 1531-1538, Jul 2010. https://doi.org/10.1109/TBME.2010.2041351

