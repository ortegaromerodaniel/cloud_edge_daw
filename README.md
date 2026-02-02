
# Tarea (c+d+e) · Edge, Fog, Mist y Cloud (DAW 1º)

## 🅲 Tarea C — Edge Computing y relación con Cloud
**Definición (3–5 líneas):**
es un nuevo paradigma de computación en el que los datos del IoT son procesados en la periferia de la red (cloud edge), en la misma fuente que los genera o tan cerca de ella como sea posible y reduce el consumo de energía, de ancho de banda y de latencia —tiempo de respuesta— que se genera al enviar tanta información a ser procesada en centros de datos remotos.

**Relación Edge ↔ Cloud (5–8 líneas):**
- Diversificación: a medida que en los próximos años el número de dispositivos IoT vaya creciendo exponencialmente, el Edge Computing será cada vez más relevante como estrategia para evitar la saturación del sistema.
- Ciberseguridad: al encontrarse la información diversificada en múltiples dispositivos, menos datos habrá en los entornos cloud y así si un entorno se ve atacado el daño será mínimo.
- Velocidad: al procesarse los datos en su lugar de origen, la inmediatez de la respuesta posibilita la existencia de herramientas como el vehículo autónomo o dispositivos de salud para emergencias.

De esta manera, el Edge Computing complementa al Cloud Computing mejorando la utilidad de los dispositivos y enviando igualmente datos a la nube para realizar análisis profundos e implementar adelantos. Asimismo, entre ambos se encuentra el Fog Computing, o computación en la niebla, que disgrega la nube en una niebla que se esparce por el mundo para estar más cerca de los dispositivos conectados, procesándose los datos no en la misma fuente sino en nodos de red cercanos.

**Ejemplo real:**
- Vehículos autónomos: Los coches inteligentes recogen información sobre su entorno mientras circulan —señales de tráfico, otros vehículos, peatones, etc.—. La velocidad de procesamiento facilitada por la computación en el borde es crucial para que los vehículos sin conductor puedan responder en tiempo real a las necesidades de la circulación y hacer viable este novedoso tipo de movilidad.

**Fuentes oficiales (mín. 2):**
- https://www.iberdrola.com/conocenos/nuestro-modelo-innovacion/que-es-edge-computing#:~:text=El%20Edge%20Computing%2C%20o%20computaci%C3%B3n,de%20ella%20como%20sea%20posible. 

## 🅳 Tarea D — Fog vs Mist (niveles y zonas de aplicación)
**Definición Fog (2–4 líneas):**
El fog computing, o computación en la niebla, es un modelo de computación descentralizado que extiende las capacidades de procesamiento y almacenamiento desde los centros de datos centrales hacia ubicaciones más cercanas a donde se generan los datos. En lugar de enviar toda la información directamente a la nube, esta arquitectura introduce una capa intermedia —la «niebla»— compuesta por nodos locales como routers, gateways o servidores periféricos que procesan y filtran los datos en tiempo real.

Este enfoque es especialmente útil en entornos donde la latencia debe ser mínima y la respuesta inmediata, como en vehículos autónomos, ciudades inteligentes o sistemas industriales conectados. Al reducir la distancia que recorren los datos, se mejora la eficiencia, se optimiza el uso del ancho de banda y se refuerza la seguridad al mantener los datos sensibles más cerca de su origen.

**Definición Mist (2–4 líneas):**
Mist Computing opera en el borde de la red. Utiliza microcontroladores, sensores y actuadores para el procesamiento local de datos. De esta manera, los datos se procesan en el mismo lugar donde se adquieren. Esto reduce la latencia y mejora las respuestas en tiempo real.
La asignación eficiente de recursos es clave para la computación en la niebla. Las tareas informáticas se ubican cerca de fuentes de datos como sensores. Esto reduce el uso del ancho de banda y la congestión de la red. El procesamiento de datos se acelera y el rendimiento de la red aumenta.

**Esquema (ASCII o Mermaid recomendado):**
[CLOUD] (Nube)
   |
   | WAN / Internet
   |
[FOG] (Nodos intermedios/Gateways)
   |
   | LAN
   |
[EDGE] (Dispositivos en el sitio)
   |
   |
[MIST] (Microcontroladores/Sensores)
   |
[IoT] (Datos)


**Zonas de aplicación (qué hace cada capa):**
- Mist → Máxima inmediatez y automatización local. Ideal para respuestas de microsegundos, reduciendo la carga de red a cero.
- Edge → Analiza y filtra datos localmente para decisiones rápidas, evitando enviar información innecesaria a la nube.
- Fog → Gestiona, agrega y analiza datos de múltiples dispositivos Edge, ofreciendo un equilibrio entre la baja latencia y la capacidad de cómputo, útil para redes IoT.
- Cloud → Almacenamiento a largo plazo, análisis de grandes volúmenes de datos (Big Data), IA y gestión global de la infraestructura. 

- https://www.arsys.es/blog/fogcomputing#:~:text=El%20fog%20computing%2C%20o%20computaci%C3%B3n,donde%20se%20generan%20los%20datos. 
- https://www.sinsmarts.com/es/blog/what-is-mist-computing/?srsltid=AfmBOooC-1xqXJK7GlsjqWkLBZKFupDY5ic4FltLC8C80sBLlrMFuM88 

## 🅴 Tarea E — Ventajas de la Cloud en sistemas conectados
Incluye mínimo 3 ventajas (recomendado 5), con explicación + ejemplo.

1) Ventaja: Ahorro de costes
   Explicación: Se elimina la necesidad de comprar servidores y hardware físico (CAPEX). Se pasa a un modelo de pago por uso (OPEX), abonando solo por la capacidad utilizada.
   Ejemplo: Una startup utiliza AWS o Azure para alojar su base de datos, evitando gastar miles de dólares en servidores físicos.

2) Ventaja: Escalabilidad y flexibilidad
   Explicación: Los recursos (almacenamiento, potencia) se pueden aumentar o disminuir en minutos según la demanda, evitando pagar recursos innecesarios.
   Ejemplo: Una tienda online aumenta su capacidad de servidor automáticamente durante el Black Friday y la reduce al finalizar la campaña.

3) Ventaja: Accesibilidad y colaboración
   Explicación: Acceso a información y aplicaciones 24/7 desde cualquier lugar y dispositivo con internet, facilitando el trabajo remoto.
   Ejemplo: Equipos utilizando Google Docs o Google Sheets para editar un informe simultáneamente desde diferentes países.

**Fuente oficial (mín. 1):**
- ...

## 📚 Fuentes (enlaces oficiales)
(Recopila aquí todos los enlaces oficiales usados)

- https://www.iberdrola.com/conocenos/nuestro-modelo-innovacion/que-es-edge-computing#:~:text=El%20Edge%20Computing%2C%20o%20computaci%C3%B3n,de%20ella%20como%20sea%20posible. 
- https://www.arsys.es/blog/fogcomputing#:~:text=El%20fog%20computing%2C%20o%20computaci%C3%B3n,donde%20se%20generan%20los%20datos. 
- https://www.sinsmarts.com/es/blog/what-is-mist-computing/?srsltid=AfmBOooC-1xqXJK7GlsjqWkLBZKFupDY5ic4FltLC8C80sBLlrMFuM88 
