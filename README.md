\[!\[Open in MATLAB Online]

# Proyecto: Sistema Lacrimal

## Información de los estudiantes

Gonzalez Sanchez Paola [22211757]; l22211757@tectijuana.edu.mx

Modelado de Sistemas Fisiológicos

Ingeniería Biomédica

## Docente

Dr. Paul Antonio Valle Trujillo; paul.valle@tectijuana.edu.mx

Departamento de Ingeniería Eléctrica y Electrónica, Tecnológico Nacional de México/IT Tijuana, Blvd. Alberto Limón Padilla s/n, Tijuana, C.P. 22454, B.C., México.

## Descripción de la asignatura

El modelizado de sistemas fisiológicos es una herramienta importante en Ingeniería Biomédica, permite comprender el funcionamiento del cuerpo humano, así como diseñar y evaluar terapias y dispositivos médicos; se define como el proceso de formular modelos matemáticos o computacionales que representan el comportamiento y la interacción de los sistemas biológicos y fisiológicos. Esta asignatura pretende aportar al perfil del Ingeniero Biomédico la capacidad de realizar investigación científica en el área de Biología de Sistemas con la finalidad de dirigir y participar en equipos de trabajo interdisciplinarios en contextos nacionales e internacionales, así como de proporcionar soluciones informáticas para resolver problemas en el campo de la Ingeniería Biomédica con ética profesional; lo anterior al proporcionar al estudiante bases sólidas para modelizar sistemas y diseñar controladores para la solución de problemas en las áreas de atención médica y del sector industrial médico. La construcción de analogías entre circuitos eléctricos y sistemas fisiológicos para la formulación de modelos matemáticos y el diseño de controladores mediante la experimentación in silico brindan herramientas de gran aplicación en el quehacer profesional del Ingeniero Biomédico.

La asignatura de Modelado de Sistemas Fisiológicos forma parte del plan de estudios de la carrera en Ingeniería Biomédica con la siguiente competencia general del curso: Utiliza las propiedades de los circuitos RLC para describir la dinámica de sistemas fisiológicos, obtener modelos matemáticos y aplicar el control clásico, esto con el objetivo de integrar los principios de la Ingeniería de Control, la Electrónica Analógica y las Ciencias de la Computación con la Anatomía y Fisiología del cuerpo humano para proporcionar descripciones cuantitativas y cualitativas de sistemas fisiológicos complejos con el objetivo de modelizar, analizar, controlar, ilustrar y predecir su dinámica tanto en el corto como en el largo plazo.

## Objetivos
1.Desarrollar el Modelo Matemático: Obtener y documentar las Ecuaciones Integro-Diferenciales del circuito RLC que modela el sistema lagrimal.

2.Determinar la Función de Transferencia: Calcular la Función de Transferencia del sistema en lazo abierto, relacionando la producción lagrimal con el volumen acumulado en el saco.

3.Analizar la Estabilidad del Sistema: Determinar la estabilidad del modelo RLC y calcular las raíces (polos) del polinomio característico para los casos Sano, Obstrucción Parcial y Obstrucción Severa.

4.Evaluar la Respuesta Dinámica: Clasificar el tipo de respuesta (amortiguamiento) para los tres casos fisiológicos y calcular el error en estado estacionario en lazo abierto.

5.Simular el Sistema en Lazo Abierto: Implementar la emulación del sistema lagrimal en SIMULINK/SIMSCAPE para obtener las curvas de respuesta transitoria y estado estacionario para cada caso.

6.Diseñar el Controlador PID: Sintonizar las ganancias de un controlador PID para el caso de Obstrucción Severa, basándose en la estabilidad y las características del sistema de segundo orden.

7.Evaluar el Desempeño del Control: Demostrar cómo el sistema en lazo cerrado (con el controlador PID) elimina el error en estado estacionario y mejora significativamente la respuesta transitoria en los casos patológicos.

8.Ilustrar Resultados Computacionales: Generar y presentar las curvas de respuesta en un cuaderno computacional de MATLAB que compare la respuesta en lazo abierto vs. lazo cerrado.

9.Crear el Diagrama Fisiológico: Diseñar un modelo fisiológico visual en BioRender que establezca una correspondencia clara entre los componentes RLC y las estructuras anatómicas del sistema lagrimal.

Documentar y Presentar el Proyecto: Elaborar un ensayo gráfico que presente de manera concisa y coherente el modelo, el análisis matemático, la sintonización del PID y los resultados de la simulación.

## Descripción detallada del sistema

El sistema lacrimal consiste en la producción de lágrimas por la glándula lagrimal, su distribución sobre la superficie ocular y su eliminación mediante el aparato de drenaje (puncta, canalículos, saco lagrimal y conducto nasolagrimal).

El sistema lagrimal, compuesto por la producción de lágrimas y el aparato de drenaje, se traduce al dominio eléctrico mediante la siguiente analogía:
Ve​(t) (Entrada),Producción Lagrimal,Tasa de entrada constante de líquido al sistema.
C (Capacitor),Saco Lagrimal (Capacitancia),Modela la capacidad de almacenamiento y distensibilidad del saco.
Rd​ (Resistencia de Drenaje),Conducto Nasolagrimal,Modela la resistencia principal al flujo de salida (Obstrucción).
L (Inductor),Flujo del Líquido,Modela la inercia y viscosidad del flujo.
Vout​(t) (Salida),Volumen/Presión en el Saco,Representa la acumulación de lágrimas (Epífora).

Se analizan tres condiciones fisiológicas, modificando los parámetros $R_d$, $C$, y $L$ para simular el grado de obstrucción:

Caso,Rd​ (Resistencia al Drenaje),C (Capacitancia del Saco),Dinámica Resultante
Sano (Control),10kΩ,2μF,"Respuesta rápida, drenaje eficiente, sin acumulación."
Obstrucción Parcial,50kΩ,1μF,"Drenaje lento, mayor tiempo de estabilización, lagrimeo ocasional."
Obstrucción Severa,100kΩ,0.5μF,"Drenaje casi nulo, acumulación crónica, tiempos de vaciado prolongados."

Palabras clave: Modelado de Sistemas; Analogía Eléctrica; Dacriocistitis; Epífora; Sobreamortiguado; Función de Transferencia; Saco Lagrimal; Controlador PID; Error de Estado Estacionario; Resistencia de Drenaje; Lazo Cerrado; Sintonización PID; Polos del Sistema; Simulink; Respuesta Transitoria.

## Lista de archivos incluidos en el repositorio

1. Cuaderno computacional de MATLAB \[.mlx].
2. Modelo de Simulink \[.slx].
4. Imagen con los parámetros del controlador.
5. Imágenes de las simulaciones \[.pdf y .png].
6. Evidencia del análisis matemático: función de transferencia, error en estado estacionario y estabilidad en lazo abierto.

## Referencias

\[1] P. A. Valle, Syllabus para Modelado de Sistemas Fisiológicos, Tecnológico Nacional de México / Instituto Tecnológico de Tijuana, Tijuana, B.C., México, 2025. Permalink: https://biomath.xyz/course/

\[2] M. C. Khoo, Physiological Control Systems Analysis Simulation, and Estimation, 2nd ed. Piscataway, New Jersey, USA: IEEE Press, 2018, Section 4, Page 93.

\[3] N. S. Nise, Control Systems Engineering, 8th ed. Hoboken, New Jersey, USA: John Wiley \& Sons, 2020.

