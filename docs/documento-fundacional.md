# EurekaMS — Mind Services
**Documento Fundacional · Versión 1.1 · Junio 2026**

---

## POR QUÉ ESTAMOS AQUÍ

El negocio mexicano opera ciego.

No porque le falte talento o ambición. Porque la información que necesita para tomar mejores decisiones existe — dispersa en su ERP, en los números de sus tiendas, en el territorio donde compite — y nadie la ha convertido en algo accionable.

En biología, la especie que sucede a la anterior no lo hace porque sea más grande, más fuerte, o más numerosa. Lo hace porque procesa información de su entorno de manera más eficiente. Los eucariotas desplazaron a los procariotas porque podían hacer más con el mismo presupuesto de energía. Los organismos con sistema nervioso central desplazaron a los que operaban por señalización química difusa porque centralizar el procesamiento de información confiere ventajas que la difusión no puede igualar.

El mecanismo es siempre el mismo: quien ve más, más rápido, con menos fricción, define el siguiente estado del sistema.

Los negocios no son diferentes. Y estamos en el momento donde esa regla se vuelve determinante.

La oportunidad que se pierde en el día a día no es dramática. No es una crisis. Es silenciosa: el SKU que debería haber estado disponible el fin de semana de mayor afluencia, la tienda que lleva seis meses underperforming sin que nadie haya hecho la pregunta correcta, la zona donde tu competidor entró primero porque nadie modeló el mercado, el prospecto que llamó el martes a las 7 PM y nadie respondió porque el equipo ya había salido.

Cada uno de esos eventos parece menor. En conjunto, son la diferencia entre un negocio que crece y uno que sobrevive.

**EurekaMS (MS = Mind Services)** existe para cerrar esa brecha. No como una consultora que entrega un reporte y desaparece. Como una capa de inteligencia que vive dentro de tu negocio, ve lo que tú no ves, y opera las oportunidades antes de que se pierdan.

---

## EL GAP QUE CUBRIMOS

Las empresas mexicanas de retail y servicios con 10 a 500 tiendas están atrapadas entre dos mundos:

**El mundo grande:** SAP, Salesforce, equipos de analytics con 8 personas. Fuera de alcance — en costo, en tiempo de implementación, en capacidad interna para operarlo.

**El mundo pequeño:** Excel, WhatsApp, intuición del director. Funciona hasta que deja de funcionar.

En medio, hay un vacío enorme.

Los sistemas existen, los datos también. Pero nadie los está convirtiendo en visión de negocio. Nadie está automatizando las interacciones repetitivas que drenan energía del equipo. Nadie está modelando el territorio antes de que el director comercial tome una decisión de expansión basada en un recorrido de campo.

EurekaMS llena ese vacío de dos maneras: con la biblioteca que ya existe y que nadie ha conectado a tu negocio — 6.1 millones de establecimientos económicos, datos demográficos por AGEB, inteligencia territorial de México entero — y con la capacidad de hacer preguntas en lenguaje natural y recibir respuestas en segundos, no en semanas.

**Las tres capacidades que antes requerían presupuestos de empresa grande:**

1. **VER** — convertir los datos de tu negocio en respuestas en lenguaje natural, sin DBA, sin tickets, sin esperar
2. **PROSPECTAR** — llegar a clientes y mercados con voz AI que escala sin contratar
3. **EXPANDIR** — decidir con evidencia dónde crecer y dónde no arriesgar

---

## CÓMO LO HACEMOS

No construimos desde cero. Integramos y especializamos un stack de tecnología que ya existe y ya funciona — lo empaquetamos para tu industria, lo conectamos a tus datos, y lo operamos contigo.

### PILAR 1: INTELLIGENCE OPS — "Tu analista de datos disponible 24/7"

Intelligence Ops conecta un agente AI directamente a tu warehouse (Postgres, Snowflake, BigQuery, SAP). El agente lee tu schema, entiende tu negocio, escribe el SQL, lo ejecuta, y te entrega la respuesta con el chart y la narrativa — en 60 segundos, por WhatsApp o en una interfaz web.

**Preguntas que responde hoy:**
- "¿Cuál es mi tienda con mayor riesgo de quiebre de stock este fin de semana?"
- "¿Qué SKUs no rotan en el norte del país desde hace 30 días?"
- "¿Por qué la tienda del Pedregal vende 40% más que su par en Satélite?"
- "¿Qué me está pidiendo el territorio que yo no estoy comprando?"
- "Dame las 10 SKUs con mayor delta entre sell-through y compra este trimestre."

Cada respuesta viene con el SQL visible y auditable. No es una caja negra — es un analista que te muestra su trabajo.

Más allá de las preguntas: el sistema genera alertas proactivas. Si detecta una anomalía (quiebre inminente, underperformance sostenida, concentración de inventario en una región que no vende), te avisa antes de que el daño ya esté hecho.

**Tecnología:** Wilab (agente MCP-nativo, whitelabel) + DENUE Analyzer + warehouse del cliente.

---

### PILAR 2: VOICE SOLUTIONS — "El vendedor que nunca duerme"

Voice Solutions automatiza las conversaciones de volumen — sin bajar la calidad, sin sonar a robot — para que tu equipo humano concentre su energía en los cierres que realmente necesitan atención personal.

**Lo que puede hacer:**
- **Inbound:** atender llamadas de clientes a cualquier hora (disponibilidad, precios, agendamiento, soporte básico)
- **Outbound:** campañas de reactivación, recordatorios de cita, seguimiento post-compra
- **Prospección:** llamadas en frío a volumen que ningún equipo humano puede igualar

El motor es PipeSong — Voice AI self-hosted con latencia menor a 1.1 segundos, costo menor a $0.03/minuto. No es una API de tercero que encarece con el volumen: es infraestructura propia que escala sin que el costo escale proporcionalmente.

---

### PILAR 3: TERRITORY OPS — "Ve el tablero antes de mover la pieza"

Territory Ops conecta 6.1 millones de establecimientos económicos (DENUE/INEGI) a tu pregunta específica.

**Preguntas que responde:**
- "¿Dónde debería abrir mi próxima tienda en CDMX?"
- "¿Qué tan saturado está el mercado de calzado deportivo en Monterrey norte?"
- "¿Cuál es el perfil socioeconómico del radio de 2km alrededor de este local?"
- "¿Qué competidores operan en esa zona y cuánto tiempo llevan ahí?"

La diferencia: mientras el estudio de mercado tradicional tarda semanas, Territory Ops responde en minutos con datos reales del tejido económico del país.

No elimina el juicio del director. Lo amplifica con evidencia.

---

## EL STACK

| Componente | Rol | Pilar |
|---|---|---|
| **Wilab** | Agente analítico MCP-nativo, whitelabel. SQL auditable. Datos en tu infra. | Intelligence Ops |
| **PipeSong** | Motor de voz AI self-hosted. Latencia <1.1s. <$0.03/min. Español nativo. | Voice Solutions |
| **DENUE Analyzer** | 6.1M establecimientos INEGI. Por zona, categoría, densidad competitiva. | Intelligence Ops + Territory Ops |
| **Mexico Uncharted** | Datos territoriales: demográficos, socioeconómicos, geoespaciales por AGEB. | Territory Ops |
| **Jarvis** | Inteligencia interna autónoma: prospecta, enriquece, detecta oportunidades. | Prospección |

---

## EL BOTTOM LINE

Los negocios que ganen la próxima década no serán necesariamente los que tengan más capital o más gente. Serán los que vean más rápido.

Los que detecten la anomalía operacional antes de que se convierta en pérdida.
Los que identifiquen el territorio antes de que lo tome la competencia.
Los que respondan al prospecto a las 7 PM del martes.
Los que conviertan los datos que ya tienen en decisiones, no en reportes.

EurekaMS es esa capa de visión.

No reemplazamos al director comercial ni al equipo de operaciones. Los movemos upstream: de ejecutar a ciegas a decidir con evidencia. De perseguir lo que ya se perdió a operar lo que aún está disponible.

La oportunidad que se pierde por falta de visión no se recupera. La que se captura con inteligencia se convierte en ventaja compuesta.

Eso es lo que construimos.

---

## PARA QUIÉN ES ESTO

**Perfil ideal:**
- Retail, servicios o food service · 10 a 500 tiendas en México
- Tiene datos (ERP, CRM, SQL, Snowflake) pero no los convierte en decisiones
- Tiene volumen de contacto que su equipo no puede procesar completamente
- Está creciendo o quiere crecer con evidencia, no con intuición

**Lo que NO somos:**
- No somos una consultora que entrega un reporte y desaparece
- No somos un software que el cliente implementa solo
- No somos un call center externo

Somos la capa de inteligencia que vive dentro de tu negocio.

---

*EurekaMS · Mind Services · Una empresa EurekaMD-net · Junio 2026*
