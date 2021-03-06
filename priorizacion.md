

![](./assets/Tapa - Priorizacion.png)

# **Saber qué es lo importante... es lo importante**

 Un consultor amigo siempre decía que las metodologías ágiles no son más que un compendio de prácticas para reducir el riesgo. En este sentido, desarrollar las funcionalidades más importantes primero es fundamental, ya que muy probablemente el dinero no alcance para todas las que el cliente desea. Al usar un proceso de desarrollo iterativo e incremental, podemos hacer _releases_ tempranos que las implementen, dejando el resto para otros posteriores. De esta manera, optimizamos el retorno de inversión y minimizamos el riesgo del proyecto.

¿Cuál es la funcionalidad más importante? El _Product Owner_ y todas las personas vinculadas al negocio seguramente conocen mejor la funcionalidad que aporta más valor, en otras palabras, la que generará mayores ingresos, resolverá más problemas u optimizará los procesos más importantes. Este no es el único factor que debemos tener en cuenta al priorizar. Otro, sumamente importante, es el riesgo tecnológico. Debemos "atacar" rápidamente todas las áreas tecnológicas que provoquen mayor incertidumbre, ya que, si no pudiésemos resolver los problemas del modo imaginado, esto podría provocar que el producto final no aportase el valor de negocio inicialmente esperado. Reducir el riesgo tecnológico también es un factor preponderante a la hora de priorizar.

Es importante que todo el equipo colabore en la priorización del producto. El _Product Owner_ será, sin embargo, el actor más importante, quien determine lo que el negocio espera. Por su parte, el equipo técnico debe colaborar activamente, identificando los riesgos tecnológicos y las dependencias. La priorización, así como el diseño, debe ser el resultado de la colaboración del equipo en pos de un objetivo compartido.

El trabajo de priorización no concluye con la escritura del _Backlog_ preliminar. Desde el inicio de su construcción, se genera un grado de conocimiento que puede impactar en la prioridad de las funcionalidades planeadas. También pueden tener lugar eventos externos \(como un anuncio de un competidor o un cambio en un proveedor\) que modifiquen nuestro plan. El _Backlog_ será la herramienta utilizada para reflejar todas las decisiones de priorización tomadas durante el transcurso del proyecto.

En este capítulo, trataremos principalmente la priorización dentro del contexto de desarrollo de un producto nuevo, transmitiendo los factores a tener en cuenta y algunas herramientas utilizadas.

# **¿Qué debe tenerse en cuenta al priorizar?**

El factor más importante es el valor de negocio, que, en su acepción más sencilla, implica cuánto dinero ganaremos. Sin embargo, este podría no llegar a ser tan directo. Existen otras aristas que influyen, como ganar nuevos clientes o una porción de mercado donde no existan otros competidores. En definitiva, **el valor de negocio que una funcionalidad entrega es el beneficio que la organización obtiene a partir de él**. Nuestro objetivo debe ser maximizarlo.

El 2do factor a tener en cuenta es el riesgo tecnológico. Si existieran componentes, _frameworks_ o servicios, que no sabemos cómo funcionan, es importante despejar esta incertidumbre lo más rápido posible. No deseamos progresar en el desarrollo del producto para luego darnos cuenta de que algo no va a funcionar y que, en consecuencia, el valor entregado sea inferior al esperado. En el mundo ágil dicen falla rápido \("_fail fast_"\) o, para decirlo en otras palabras tomadas de Alistair Cockburn, aprende rápido \("_learn fast_"\).

Otra perspectiva desde la que podemos mirar este tópico de priorización es la del aprendizaje. Estamos aprendiendo y debemos lidiar con riesgos e incertidumbres. En consecuencia, deberíamos priorizar todo aquello que nos permita aprender.

Otro factor que podríamos llegar a tener en cuenta, aunque de menor importancia, es el esfuerzo \(o costo\). Conociéndolo, el _Product Owner_ podrá decidir que una funcionalidad es demasiado costosa para el valor que arroja o, por el contrario, construir otra menos valiosa, solamente porque el esfuerzo requerido es menor. Para ponerlo en términos formales, la razón costo-beneficio puede influir en la priorización.

Ninguno de estos factores decide la priorización por sí mismo, ya que tanto los de negocios, como los tecnológicos, deben ser tenidos en cuenta. Como ya mencioné anteriormente, las decisiones de priorización serán el resultado de la colaboración entre todas y todos.

# ***Releases* cortos**

Antes de interiorizarnos en muchas de las herramientas utilizadas, les mostraré la heurística más importante a la hora de priorizar y de planear. Acoten, tanto como sea posible, la cantidad de trabajo. En otras palabras, en lugar de hacer _releases_ grandes y riesgosos, háganlos simples y breves. Les resumo las ventajas que obtendrán:

* **Maximiza el retorno de inversión del proyecto**: Desde el punto de vista financiero, no hay dudas de que es sumamente beneficioso, ya que, en un periodo de tiempo mucho menor, obtendremos parte del valor de negocio prometido \(que puede ser usado para financiar el resto del proyecto\).
* **Minimiza el riesgo**: Tener mucho trabajo en progreso representa un riesgo, porque las condiciones \(internas o externas\) pueden cambiar. Al construir el MVP, debemos acotar este _release_ al mínimo posible, para testear la hipótesis única de valor \(que tiene un riesgo muy grande\) al menor costo posible.
* **Minimiza la incertidumbre**: No olvidemos que, antes de construir el producto y testearlo con usuarios reales, sólo hipotetizamos. 

Verán menciones a esta heurística en toda la literatura ágil. Kent Beck incluyó, entre las reglas de planeamiento de _eXtreme Programming_, una que denominó ''[releases cortos y frecuentes](http://www.extremeprogramming.org/rules/releaseoften.html)''[[Beck00]](bibliografia.md#beck00-beck-kent-fowler-martin-planning-extreme-programming-the-xp-series-octubre-2000). Probablemente fue quien luego propició uno de los [principios ágiles](http://agilemanifesto.org/principles.html) que afirma: "buscamos satisfacer a los clientes a través de la entrega continua de software con valor". La [declaración de interdependencia](http://pmdoi.org/), escrita por _Project Managers_, específica que "se aumenta el retorno de inversión, haciendo foco en tener un flujo continuo de valor". Las reglas de [Lean Software Development](https://en.wikipedia.org/wiki/Lean_software_development) [[Poppendieck00]](bibliografia.md#poppendieck00-poppendieck-00-mary-tom-lean-software-development-an-agile-toolkit-mayo-2003) van en la misma dirección. Una de ellas proclama: "debemos entregar software rápidamente, ya que implica una ventaja competitiva". Finalmente, [Kanban](https://www.crisp.se/gratis-material-och-guider/kanban) [[Anderson00]](bibliografia.md#anderson00-anderson-david-kanban-successful-evolutionary-change-for-your-technology-business-abril-2010) [[Kniberg00]](bibliografia.md#kniberg-00-kniberg-henrik-lean-from-the-trenches-managing-large-scale-projects-with-kanban-diciembre-2011) hace de todo esto su _leit motiv_. Sus reglas principales comprenden "visualizar el flujo de valor", para "limitar el trabajo en progreso" y, de esta manera, "maximizarlo".

En estos días, muchos de nuestros clientes, que ya poseen un producto en funcionamiento, usan [_continuous delivery_](https://continuousdelivery.com/). El precepto es el mismo. De este modo, agregan valor diariamente o, incluso, varias veces en un día. Los _releases_ pequeños y frecuentes de los que hablaba Beck en los años 90 se llevaron al extremo.

Ahora sí, veamos algunas de las herramientas que usamos frecuente en distintas etapas del proceso de priorización.

# **Herramientas**

Utilizo frecuentemente las herramientas que a continuación describiré porque permiten visualizar y facilitar el proceso de priorización. Además, resultan simples para entender y livianas de implementar. Existen otras más sofisticadas, por ejemplo las financieras, que calculan el retorno de inversión, sobre las que no profundizaré aquí.

Empezaré por el _User Story Map_, detallando su empleo a la hora de priorizar, durante el _Product Discovery_. Seguiré con una herramienta extremadamente simple, pero muy útil al mismo tiempo, llamada MoSCoW. A continuación, les mostraré otras, pensadas para la visualización de la razón costo-beneficio y finalmente terminaré con otra, llamada _product roadmap_, muy útil a la hora de facilitar la priorización de funcionalidades nuevas para un producto ya implementado.    
****

## ![](.gitbook/assets/32x32.png) _**User Story Mapping**_

Esta herramienta nos permite visualizar el producto completo rápidamente, resultando de gran utilidad para facilitar la priorización. Lo usamos durante las sesiones de _Product Discovery_, ya que posibilita la comprensión del orden de importancia de las tareas detectadas y también el conjunto mínimo necesario para una versión inicial.

Como ya vimos en el [capítulo 1](product-discovery.md), la manera de indicar que una tarea resulta más importante que otra consiste en situarla sobre la de menor importancia. Esta decisión siempre es precedida por interesantes discusiones plasmadas, de modo visual, en el _story map_.

El _User Story Map_ es una herramienta muy útil también para decidir cuál será el MVP, es decir, el producto que nos permite testear la hipótesis única de valor. Simplemente trazamos una línea por debajo de todas las tareas incluidas en él. Aquellas, situadas por sobre ésta, representan el MVP. Frecuentemente, vemos una gran cantidad de *post-its* por sobre la línea, lo que nos permite comprender, instantáneamente, que el MVP seleccionado es demasiado grande. En esos casos, procuramos mover la línea hacia arriba. Como ya mencioné en la sección anterior, prefiero _releases_ cortos.

![](./assets/priorizacion-user-story-mapping.png)

Soy un fan de esta herramienta. Todas las conversaciones empleadas en la toma de estas decisiones tienen lugar frente al "mapa" del producto, quedando inmediatamente plasmadas.    
****

## ![](.gitbook/assets/32x32.png) ***MoSCoW***

Esta técnica de priorización es la más sencilla de todas. Consiste en categorizar las _User Stories_ o las épicas según su importancia. Las categorías, cuyas iniciales dan nombre a la técnica, son:

* _Must_: Las obligatorias.
* _Should_: Deberían estar.
* _Could_: Podrían estar.
* _Won’t_: No van a estar.

Pese a su simpleza, esta herramienta resulta sumamente útil, ya que nos obliga a consensuar, entre todo el equipo, una categoría para cada uno de los ítems.

Podemos usarla para priorizar un conjunto de _User Stories_ o épicas de un producto nuevo y también funcionalidades que deseamos agregar a uno en funcionamiento. Un ejemplo muy interesante de esta última situación tuvo lugar dentro de un equipo con el que colaboré: 3 _Product Owners_ debían priorizar las épicas del bimestre venidero. Resultó muy interesante observar cómo reconocían la imposibilidad para completar el trabajo, al visualizar la gran cantidad de épicas categorizadas en "_Must_", y decidían las que podían posponerse. Como ya les mencioné, la utilidad de la herramienta yace en que **obliga a un conjunto de personas a consensuar categorías para un conjunto de ítems de un modo muy visual**.

Con este equipo, solíamos priorizar también las épicas de cada categoría, sobre todo, las de la categoría "*Must*". Así lográbamos categorizar las épicas por bimestre, así como también conocer el orden de las que desarrollaríamos próximamente.    
****

![](./assets/moscow.png)

## ![](.gitbook/assets/32x32.png) **Puntos de valor de negocio**

Otra herramienta de gran utilidad durante el proceso de priorización es la asignación de "puntos de valor de negocio" \(_business value points_\) a las diferentes funcionalidades, haciendo una comparación similar a la utilizada al estimar _Story Points_ pero, esta vez, **asignando valores relativos en lugar de esfuerzos relativos**. Las piezas de funcionalidad a las que asignamos puntos deben ser necesariamente mayores que las _User Stories_, ya que estas últimas, por sí mismas, son unidades funcionales muy pequeñas para representar un valor de negocio.

Como en la técnica de *MoSCoW*, también nos fuerza a consensuar y explicitar valores. Decimos que una épica es más importante que otra, pero ¿cuánto? ¿estamos de acuerdo en eso? Explicitar esos puntos de valor de negocio puede resultar un ejercicio muy fructífero. Además, una vez estimados el valor y el esfuerzo, podemos establecer la razón costo-beneficio de cada una de ellas. 

Existen varios modos de visualización, que transmitiré mediante el ejemplo del sistema para el cajero de supermercados del capítulo 1. Imaginen que necesitamos agregar las épicas que presento a continuación, a las cuales asignaremos los siguientes puntos de valor de negocios y esfuerzo. Obtendremos  algo similar a la tabla siguiente:    

****

| **Épica** | **Valor de Negocios** | **Puntos de Esfuerzo** | **Razón \(Beneficio\)** |
| :--- | :--- | :--- | :--- |
| **Pago con Bitcoins** | **2** | **1** | **2** |
| **Pago con Tarjeta de Descuentos** | **5** | **3** | **1.66** |
| **Reportes en Tiempo Real para Jefes** | **8** | **5** | **1.6** |

La 4ta columna es la razón entre el valor de negocios y los puntos de esfuerzo, es decir, la división entre el valor de la 2da columna y de la 3ra. Aquí se puede ver como la épica más beneficiosa es "Pago con Bitcoins", con un beneficio de 2. El valor de negocios es el más pequeño, pero el esfuerzo también. El _Product Owner_ podría decidir priorizar "la fruta que cuelga baja en el árbol" ([_low hanging fruit_](https://www.merriam-webster.com/dictionary/low-hanging%20fruit)). Paradójicamente, la épica menos beneficiosa es la de mayor valor de negocios, justamente porque implica un esfuerzo importante.

En mi experiencia, el costo es un factor sustancialmente menos importante que los demás \(valor de negocios y riesgo\). En contadas ocasiones observé a un _Product Owner_ tomar la decisión de priorizar una funcionalidad solamente porque su desarrollo no fuera costoso. Para resolver esto, podemos añadir "pesos" para cada uno de los factores. Siguiendo el ejemplo anterior, si especificáramos un peso de 0.7 para el valor de negocios y 0.3 para el esfuerzo, obtendríamos los siguientes resultados.    
****

| **Épica** | **Valor de Negocios \(0.7\)** | **Puntos de Esfuerzo \(0.3\)** | **Razón \(Beneficio\)** |
| :--- | :--- | :--- | :--- |
| **Pago con Bitcoins** | **2 \[1.4\]** | **1 \[0.3\]** | **4.66** |
| **Pago con Tarjeta de Descuentos** | **5 \[3.5\]** | **3 \[0.9\]** | **3.88** |
| **Reportes en Tiempo real para Jefes** | **8 \[5.6\]** | **3 \[0.9\]** | **6.22**  |

[Jim Highsmith](https://g.co/kgs/dNXTTD) argumenta la visualización de los beneficios como porcentajes ya que esto prevendría que, al trabajar con diferentes equipos, se exageren los puntos de valor. Los resultados para el ejemplo serían los que presento a continuación, donde calculamos el porcentaje de valor para cada una de las épicas, el porcentaje de esfuerzo y luego la razón.    

****

| **Épica** | **Valor de Negocios \(0.7\)** | **% de Valor** | **Puntos de Esfuerzo \(0.3\)** | **% de Esfuerzo** | **Razón \(Beneficio\)** |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **Pago con Bitcoins** | **2** | **0.13** | **1** | **0.14** | **0.92** |
| **Pago con Tarjeta de Descuentos** | **5** | **0.33** | **3** | **0.42** | **0.78** |
| **Reportes en Tiempo Real para Jefes** | **8** | **0.53** | **3** | **0.42** | **1.26** |
| **Total** | **15** |  | **7** |  |  |


Todas las técnicas mostradas son similares, ya que nos fuerzan a explicitar valores y esfuerzos y nos devuelven un indicio de lo que podría ser la funcionalidad de mayor beneficio. Pueden incluso agregarse columnas, modificando consecuentemente la fórmula, para incorporar otros factores, por ejemplo, una penalidad \(si la épica no fuera desarrollada\) o el riesgo \(como en el ejemplo del _paper_ de [Karl Wiegers](http://www.processimpact.com/articles/prioritizing.pdf)\). En definitiva, el valor de la herramienta consiste en que fuerza a volcar toda la subjetividad existente en nuestras cabezas sobre una tabla con números explícitos, que calculan un beneficio a través de una fórmula acordada.

## ![](.gitbook/assets/32x32.png) ***Tracer Bullets***

Cuando empezamos con un producto nuevo, el equipo técnico debe pensar cómo encarar su desarrollo, es decir, cómo construir el producto mínimo viable iterativa e incrementalmente y cómo testear que la arquitectura y tecnologías elegidas soporten los requerimientos funcionales y no funcionales. En esta fase de la priorización, de más bajo nivel, nos centramos en atacar los riesgos e incertidumbres y en dividir el trabajo de la mejor manera.

Con este objetivo, elegimos un conjunto de _User Stories_ que nos permitan construir el esqueleto de la aplicación, los componentes que representan la arquitectura de la misma. En esta etapa, ponemos énfasis en la parte iterativa del proceso de desarrollo. Nos enfocamos en la obtención de un esqueleto visible que pruebe los componentes principales y dejamos los incrementos para más adelante. Esta heurística es lo que Andy Hunt y Dave Thomas llaman una Bala Trazadora o [_Tracer Bullet_](http://www.artima.com/intv/tracer.html).

Esta _Tracer Bullet_ permite testear todas las capas de nuestra arquitectura y crear una columna vertebral a partir de la cual hacer incrementos de funcionalidad. Además, nos permite mostrar un avance al usuario rápidamente \(aunque no tenga la calidad final\) y también correr tests de carga/_stress_ que validen la arquitectura elegida.

## ![](.gitbook/assets/32x32.png) ***Product Roadmap***

Esta es una herramienta utilizada por una experimentada _Product Owner_ con la que tuve la oportunidad de trabajar, para priorizar y organizar el trabajo de los próximos meses para los diferentes grupos de los que formaba parte. Después de conocerla, leí el libro *Managing your Project Portfolio*[[Rothman00]](bibliografia.md#rothman00-rothman-johanna-book-manage-your-project-portfolio-increase-your-capacity-agosto-2009), que la explica detalladamente.

Al observar la imagen siguiente, probablemente alcancen a comprender su funcionamiento. En un eje, se especifican las unidades de tiempo y, en el otro, los diferentes equipos. Luego grafican el periodo que, estiman \(de modo superficial\), consumirá cada una de las épicas que tienen priorizadas en la columna correspondiente al equipo al que se asignará.    

![](./assets/product_roadmap_horizantal_1.png)

La única herramienta digital que conozco, sin haber utilizado, es [Roadmunk](https://roadmunk.com/jira-roadmap-integration). Lo bueno de que sea un _plugin_ de [Jira](https://www.atlassian.com/software/jira) reside en que las mismas épicas planeadas en el _roadmap_ son usadas posteriormente en la herramienta de gestión, una vez iniciada la construcción.

## ![](.gitbook/assets/32x32.png)*Buy a Feature* – por Germán Gaitan

En ocasiones, el producto que estamos desarrollando impacta en diferentes áreas de la organización, cuyos objetivos y expectativas son diferentes (¡y hasta contrapuestos!). En estos casos, si los *stakeholders*, que representan estas áreas, no logran establecer un consenso acerca del valor de las funcionalidades, podemos recurrir a otras técnicas que nos permitan realizar la priorización de una manera subjetiva, pero aún colaborativa, como es el caso de *Buy a Feature*[[1]](priorizacion.md#notas-al-pie):

Cada *stakeholder* escribe las funcionalidades de su interés en tarjetas, como si se tratara de productos de góndola. Incluso pueden destinarse algunos minutos a darles un aspecto más atractivo o *marketinero* (utilizando *stickers*, colores, etc.). Una vez preparadas, las tarjetas se colocan sobre una mesa donde todas quepan de forma bien visible y se dan unos minutos para que todos las puedan leer y debatir acerca de su significado.

Entregamos a cada *stakeholder* una cantidad equitativa de fichas de póker, dinero de fantasía o hasta porotos. En mi opinión lo mejor es utilizar fichas de póker -cuanto más pesadas, mejor- ya que brindan una sensación de valor genuino. En general se da a todos la misma cantidad de fichas (5 por ronda, por ejemplo), pero pueden entregarse cantidades diferentes en función de su jerarquía en la organización o de algún otro atributo que determine lo que vale su voto.

Comienza la primera ronda. Cada *stakeholder* “gasta” sus fichas repartiéndolas entre las funcionalidades que son de su interés. Pueden aplicarse algunas restricciones, como que no deben colocarse todas las fichas en la misma funcionalidad o alguna otra variante que asegure un voto diversificado. Al término de esta fase, se cuentan las fichas de cada una. La más votada es retirada de la mesa, seleccionada como prioritaria. Si dos funcionalidades comparten el primer lugar, se espera a la siguiente ronda para definir.

La actividad se realiza en varias rondas, entregando siempre las mismas cantidades de fichas. Las tarjetas de funcionalidad que permanecieron en la mesa conservan las fichas que vienen acumulando de las rondas anteriores. En cada ronda se retira la tarjeta con más fichas y se coloca debajo de la seleccionada en la ronda anterior en orden de prioridad.

En general se realizan tres o cuatro rondas de compra de funcionalidades. Todo depende de la cantidad de participantes y de la cantidad de fichas de las que cada uno dispone. Lo que indica que ya se iteró suficiente es que, al finalizar una ronda, quedan sobre la mesa varias tarjetas con muchos votos, que pueden ser priorizadas con las fichas que sumaron hasta ese momento.

Esta experiencia suele ser divertida y muy distendida. Favorece las charlas de negociación de funcionalidades entre *stakeholders* en cada ronda. Su resultado es una priorización rápida y con altísima aceptación.

# **Priorizando experimentos**

Cuando hablamos de valor de negocio en esta etapa, en la que todavía no existe un producto, en realidad hipotetizamos sobre el potencial que, creemos, entregará. Nos queda validar estas hipótesis con usuarios reales, ¿estarán dispuestos a pagar por nuestro producto?

Haremos esto mediante experimentos, que testean si lo supuesto se cumple. Teniendo esto en cuenta, la priorización consiste en determinar el modo de testeo de las hipótesis. En otras palabras, pensar y priorizar experimentos y, de acuerdo a ésto, decidir qué funcionalidad incluir en cada uno de ellos. De este modo, el producto mínimo viable \(*MVP*\) no es más que el primero de nuestros experimentos, que valida la hipótesis única de valor.

Todos estos conceptos están tomados de la metodología de _Lean Startups_[[Ries00]](bibliografia.md#ries00-ries-eric-the-lean-startup-septiembre-2011), de Eric Ries. Planear, construir y validar con usuarios reales. Los lineamientos generales son muy similares a los de las metodologías ágiles, pero van un paso más allá.

Uno de los puntos fundamentales de esta metodología consiste en definir cómo vamos a medir el funcionamiento del experimento. De haber realizado el _Lean Canvas_, mencionado en el capítulo 1, recordarán que una de las secciones consistía en describir explícitamente estos experimentos. En muchos de los desarrollos en los que trabajé, no existía certidumbre acerca de cómo se validaría lo construido. Sin embargo, esto es fundamental, ¡debemos saber lo que se quiere lograr!

Cheryl Quirion compartía estos experimentos visualmente con todo el equipo de desarrollo, usando una técnica que denominó [Lean Visual Strategy](https://leanvisualstrategy.com/what-is-lean-visual-strategy-4b4dc9df610d). Compartir esta información con el equipo permite que esté alineado y entienda por qué lo está construyendo. Hacerlo de manera visual ayuda a que todas y todos incorporen esta información mejor y más rápidamente.

# **Conclusiones**

Realizar una buena priorización antes de empezar con el desarrollo es fundamental. Empezamos por determinar la funcionalidad necesaria para realizar el primer experimento, llamado *MVP*. Luego, el orden en que lo construiremos de manera de minimizar el riesgo y maximizar el valor.

Este camino que trazamos es creado colaborativamente y compartido por todas y todos. Las herramientas que mencioné contribuyen en el proceso. Una vez iniciada la construcción resulta fundamental mantener un _Backlog_ actualizado. Queremos estar seguros de estar trabajando, en todo momento, sobre las funcionalidades más importantes, es decir, las que aporten más valor y reduzcan más el riesgo.

# Notas al pie



1. *Buy a Feature*: Compre una funcionalidad