# Circuit Bending de Juguetes

### Electrónica Analógica y Digital · Universidad Andrés Bello

Proyecto experimental de **circuit bending** realizado como parte de la asignatura Electrónica Analógica y Digital.

La idea fue tomar juguetes electrónicos reutilizados y explorar qué ocurre cuando intervenimos sus circuitos, modificando o conectando distintos puntos para generar nuevas respuestas sonoras, eléctricas y visuales.

Más que buscar solamente "hacer que el juguete funcione distinto", nos interesó entender **por qué cambia su comportamiento** y utilizar la electrónica como una herramienta de experimentación.

Este proyecto combina simulación, análisis de circuitos, montaje físico y exploración sonora.

## Sobre el proyecto

El circuit bending es una práctica experimental que consiste en intervenir circuitos electrónicos existentes para encontrar comportamientos no previstos originalmente por el fabricante.

En nuestro caso trabajamos principalmente con juguetes electrónicos alimentados por pilas. Antes de modificar los circuitos, realizamos una etapa de observación y diagnóstico para identificar:

- alimentación y tierra;
- componentes electrónicos;
- pistas de las placas;
- botones y entradas;
- parlantes y micrófonos;
- motores;
- puntos de soldadura;
- circuitos relacionados con el sonido.

La exploración se realizó inicialmente de manera no invasiva, utilizando puentes temporales y observando cómo respondía el circuito.

A partir de estas pruebas fuimos relacionando los cambios observados con conceptos de electrónica analógica y digital vistos durante la asignatura.

## Objetivos

### Objetivo general

Explorar y modificar juguetes electrónicos mediante técnicas de circuit bending, aplicando conocimientos de electrónica analógica y digital para generar nuevas respuestas sonoras y visuales.

### Objetivos específicos

- Comprender el funcionamiento básico de los circuitos presentes en juguetes electrónicos.
- Identificar componentes y pistas en placas reales.
- Aplicar conceptos como Ley de Ohm, KCL, KVL y análisis de circuitos.
- Experimentar con resistencias, condensadores, transistores, diodos y otros componentes.
- Utilizar simuladores como Tinkercad y Proteus para complementar el análisis.
- Documentar los resultados de las intervenciones.
- Explorar la relación entre electrónica, sonido y experimentación artística.

## Enfoque de aprendizaje

Una de las ideas principales del proyecto fue aprender electrónica no solamente desde los esquemas, sino también desde circuitos reales.

Trabajar con juguetes permitió encontrarnos con placas que no necesariamente están diseñadas para ser estudiadas por estudiantes: componentes pequeños, circuitos integrados sin documentación visible, pistas difíciles de seguir y sistemas cuyo funcionamiento interno no conocemos completamente.

Por eso el proceso fue principalmente experimental:

**observar → formular una hipótesis → probar → escuchar/observar el resultado → intentar entender qué ocurrió → documentarlo.**

Los errores también forman parte del proyecto. Algunas pruebas no produjeron ningún cambio, otras generaron ruido o distorsión y otras nos ayudaron a descubrir puntos interesantes del circuito.

La documentación busca mostrar este proceso y no solamente presentar un resultado final.

## Juguetes explorados

Durante la etapa inicial trabajamos con distintos juguetes electrónicos reutilizados.

### Piano Tucán — Huanger

Juguete musical que permitió explorar principalmente el circuito asociado al sonido.

Durante las pruebas se identificó un condensador marcado como `104`, equivalente a aproximadamente `100 nF`, además de conexiones hacia el parlante y el interruptor de alimentación.

Fue el juguete donde encontramos algunas de las respuestas más interesantes al realizar puentes temporales sobre distintos puntos del circuito.

### Celular para bebés — Clementoni

El juguete presentaba un funcionamiento parcial y solamente emitía un pitido breve.

A pesar de esto, permitió observar la estructura de una placa de juguete y sus conexiones hacia botones y elementos sonoros.

### Camión Tow Truck — VTech

El juguete no respondió durante las primeras pruebas. Se observaron cables y contactos asociados a la alimentación que presentaban signos de oxidación.

En este caso, el diagnóstico también fue parte del aprendizaje: no todos los circuitos reutilizados se encuentran en condiciones de funcionamiento.

## Primera exploración de circuit bending

La primera etapa de experimentación se realizó sin soldar componentes permanentemente.

Utilizamos un cable con las puntas expuestas como puente temporal para tocar diferentes puntos de los circuitos mientras los juguetes estaban funcionando.

El objetivo era observar si aparecían cambios en:

- tono;
- volumen;
- ritmo;
- ruido;
- distorsión;
- comportamiento de los botones;
- respuesta del circuito.

### Algunas observaciones

| Prueba | Resultado |
|---|---|
| Puente entre la soldadura del switch y el componente `104` | Variación del tono y volumen, con sonido distorsionado |
| Contacto con zonas correspondientes a los botones | Activación normal de los sonidos |
| Contacto con soldaduras del parlante | Aparición de ruido e interferencia leve |
| Contacto simultáneo con varios puntos | No se observaron cambios significativos |

Estas pruebas fueron principalmente exploratorias. Las interpretaciones iniciales fueron utilizadas como hipótesis para continuar investigando el circuito.

### Sobre la interpretación de los resultados

Una de las observaciones más interesantes ocurrió al intervenir cerca del componente marcado como `104`.

El resultado fue un cambio perceptible en el tono, volumen y distorsión del sonido.

En ese momento planteamos como hipótesis que el condensador y las conexiones cercanas estaban afectando la respuesta de la etapa de audio. Sin embargo, para confirmar exactamente qué estaba ocurriendo sería necesario reconstruir o analizar con mayor detalle el circuito.

Por eso distinguimos entre lo que observamos experimentalmente y lo que todavía estamos investigando.

## Componentes y herramientas

Para las distintas etapas del proyecto utilizamos o tenemos disponibles:

### Electrónica

- Protoboard de 830 puntos
- Resistencias de distintos valores
- Condensadores electrolíticos y cerámicos
- LEDs
- Diodos
- Transistores 2N2222A / PN2222
- Potenciómetro de precisión de 10 kΩ
- Fotorresistencias (LDR)
- Termistor
- Pulsadores
- Zumbador pasivo
- Motor de vibración
- Motor DC
- 74HC595
- 4N35
- Cables jumper
- Portapilas y baterías
- Interruptores

### Herramientas

- Soldador
- Estaño
- Multímetro
- Protoboard
- Pinzas
- Destornilladores
- Cables de prueba

### Software

- Tinkercad Circuits
- Proteus
- LaTeX

## Simulación

Antes y durante la experimentación física utilizamos simuladores para comprender algunos de los circuitos que aparecen o pueden incorporarse al proyecto.

Entre las simulaciones consideradas se encuentran:

- circuitos LED + resistencia;
- divisores de voltaje;
- circuitos RC;
- transistores como interruptores;
- compuertas lógicas;
- registros de desplazamiento;
- osciladores;
- generación de señales para audio.

La simulación nos permite probar algunas ideas antes de llevarlas al circuito físico y comparar posteriormente el comportamiento esperado con el comportamiento real.

## Seguridad

El proyecto se realiza utilizando circuitos de baja tensión.

Como regla general:

- trabajamos con juguetes alimentados por pilas;
- evitamos dispositivos conectados directamente a la red eléctrica;
- no intervenimos fuentes de alimentación de corriente alterna;
- evitamos manipular baterías de litio integradas;
- las pruebas se realizan con cuidado para evitar cortocircuitos;
- al soldar utilizamos las precauciones correspondientes;
- los circuitos se desconectan antes de realizar modificaciones físicas.

El circuit bending puede producir comportamientos impredecibles en un circuito, por lo que las modificaciones permanentes se realizan solamente después de identificar razonablemente los puntos que se quieren intervenir.

## Estado actual

**Proyecto en desarrollo / documentación en progreso.**

La primera etapa permitió familiarizarnos con los juguetes, identificar componentes y encontrar algunos puntos que producen cambios sonoros.

Actualmente estamos ampliando la exploración hacia circuitos externos y pequeños módulos electrónicos que permitan construir nuestras propias etapas de sonido.

Uno de los objetivos a futuro es pasar desde la modificación de juguetes existentes hacia la construcción de pequeños instrumentos electrónicos y módulos experimentales propios.

## Próximos pasos

- Documentar con fotografías las placas y puntos de intervención.
- Identificar con mayor precisión los componentes de los juguetes.
- Repetir las pruebas utilizando un multímetro.
- Diseñar circuitos equivalentes en Tinkercad.
- Experimentar con resistencias y condensadores para modificar señales.
- Explorar transistores como etapas de conmutación.
- Construir pequeños generadores de sonido.
- Investigar diferentes formas de obtener interacción física con los circuitos.
- Comparar simulaciones con resultados reales.
- Registrar en audio y video las modificaciones más interesantes.
- Continuar documentando los errores y resultados inesperados.

## Documentación

Este repositorio busca funcionar como una bitácora técnica del proyecto.

Aquí iremos incorporando:

- informes;
- esquemas;
- simulaciones;
- fotografías;
- diagramas;
- registros de experimentos;
- listas de componentes;
- cálculos;
- resultados;
- videos;
- reflexiones sobre el proceso.

La idea es que el repositorio pueda crecer junto con el proyecto y servir también como registro de nuestro aprendizaje en electrónica.

## Equipo

Proyecto desarrollado por estudiantes de Ingeniería en Automatización y Robótica de la Universidad Andrés Bello, en el contexto de la asignatura Electrónica Analógica y Digital.

**Integrantes:**

- Lucas Muñoz
- María José Córdova
- Benjamín Martínez
- Alex Canales Díaz

**Asignatura:** Electrónica Analógica y Digital  
**Universidad:** Universidad Andrés Bello  
**Año:** 2025

## Referencias

- Ghazala, R. (2005). *Circuit-Bending: Build Your Own Alien Instruments*. Wiley Publishing.
- Boylestad, R. L. (2015). *Introducción al análisis de circuitos*. Pearson.
- Hayt, W. H., Kemmerly, J. E. & Durbin, S. M. (2012). *Análisis de circuitos en ingeniería*. McGraw-Hill.
- Horowitz, P. & Hill, W. (2015). *The Art of Electronics*. Cambridge University Press.
- Autodesk. *Tinkercad Circuits*.
- Labcenter Electronics. *Proteus Design Suite*.

---

## Aprender haciendo

Este proyecto comenzó como una actividad para una asignatura, pero terminó convirtiéndose en una forma de acercarnos a la electrónica desde la experimentación.

Todavía hay muchas cosas que no entendemos completamente, y justamente por eso seguimos probando.

**Observar → intervenir → escuchar → medir → equivocarse → entender → volver a probar.**

Ese es, por ahora, nuestro circuito.
