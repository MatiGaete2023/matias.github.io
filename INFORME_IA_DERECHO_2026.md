# IA en el ejercicio del derecho: estado, comparativa y hoja de ruta para Chile

**Fecha de corte:** 17 de julio de 2026. **Alcance:** investigación estratégica; no sustituye asesoría jurídica, evaluación de impacto ni validación de un proveedor. Las cifras de proveedores se identifican expresamente como tales: no deben confundirse con resultados auditados de un despacho.

## Registro de ejecución y control de calidad

**Iteración 1: [Detectados vacíos: se mezclaban promesas comerciales con métricas independientes; faltaban separar analítica, IA generativa y automatización; y no estaba temporalizada la transición chilena de datos personales] -> Iteración 2: [Correcciones: se etiquetaron las métricas por fuente y método, se añadió una matriz de madurez y se precisó que la Ley N.º 21.719 fue publicada el 13 de diciembre de 2024 y entra en vigencia el 1 de diciembre de 2026] -> Iteración 3: [Pulido final: se limitaron las afirmaciones sobre adopciones chilenas a implementaciones públicas verificables, se incorporaron controles de secreto profesional/retención y se añadió una matriz de decisión para firmas boutique].**

## Resumen ejecutivo

La adopción útil de IA jurídica no es “un chatbot para abogados”. Es una arquitectura compuesta por: (1) **automatización determinista** para capturar datos, plazos y documentos repetibles; (2) **analítica predictiva/estadística** para priorizar asuntos y estimar resultados a partir de datos históricos; y (3) **IA generativa (GenAI)** para recuperar, resumir, comparar y proponer borradores con trazabilidad humana. La primera es la más madura y de menor riesgo; la tercera crea la mayor palanca de productividad y el mayor riesgo de confidencialidad, alucinación y sesgo.

La estimación pública más útil para capacidad es la de Thomson Reuters: los profesionales jurídicos encuestados estimaron que GenAI podría liberar **12 horas semanales** en cinco años. Es una expectativa de encuesta, no una garantía de reducción de horas facturables ni una medición causal. La investigación de revisión asistida por tecnología (TAR) sí muestra que los sistemas de aprendizaje activo pueden alcanzar o superar la revisión humana en recuperación/precisión bajo diseños controlados; no autoriza a prescindir de validación, protocolos de privilegio ni muestreo estadístico.

Para Chile, la ventana 2026–2027 es especialmente relevante: hasta el **30 de noviembre de 2026** rige principalmente la Ley N.º 19.628; desde el **1 de diciembre de 2026**, la Ley N.º 21.719 instala una Agencia de Protección de Datos Personales, nuevos principios, derechos y obligaciones. Un despacho que cargue expedientes a un modelo externo debe tratarlo como una operación de tratamiento: inventario, base de licitud, contrato de encargado, controles de transferencias internacionales, minimización, seguridad, retención y respuesta a incidentes. El secreto profesional no queda desplazado porque una herramienta sea “empresarial”.

## 1. Estado global del arte

### 1.1 Taxonomía práctica

| Capa | Qué hace | Ejemplos de software | Mejor caso de uso | Riesgo dominante | Control mínimo |
|---|---|---|---|---|---|
| Automatización de flujo | Reglas, formularios, tareas, alertas y plantillas | Clio Grow/Manage, Lawmatics, BRYTER, Bigle Legal, Docassemble | Intake, conflictos, poderes, expedientes y calendario | Regla mal configurada o cómputo legal erróneo | Dueño del proceso, pruebas de regresión y bitácora |
| Analítica predictiva | Infere patrones desde datos pasados; no “adivina” el derecho | Lex Machina, Bloomberg Law Litigation Analytics, Premonition | Selección de foro, duración, tasas de mociones, estrategia de cartera | Datos incompletos, causalidad aparente y perfilamiento | Fuente/cobertura documentada, intervalo de confianza y revisión del abogado |
| IA generativa y recuperación | Busca, resume, clasifica, compara y redacta texto | CoCounsel, Westlaw Precision, Lexis+ AI, Harvey, vLex Vincent AI, Noxtua | Investigación con citas, due diligence, primera versión de contrato o escrito | Cita inventada, fuga de datos, instrucción ambigua | RAG con corpus autorizado, citas verificadas y aprobación humana |
| Revisión de documentos con ML | Prioriza y etiqueta grandes poblaciones documentales | Relativity aiR, Reveal Brainspace, Everlaw | E-discovery, investigaciones, privilegio y cláusulas | Falsos negativos y pérdida de privilegio | Protocolo TAR, muestras de control y equipo de privilegio |

**Regla de diseño:** la IA no decide la posición jurídica ni firma un escrito. El abogado conserva la verificación de fuentes, juicio profesional, comunicación con cliente y responsabilidad por el producto final.

### 1.2 Métricas: qué está probado y qué no

| Métrica / resultado | Dato | Lectura correcta |
|---|---:|---|
| Capacidad potencial con GenAI | **12 h/semana** a cinco años, según profesionales jurídicos encuestados por Thomson Reuters | Percepción prospectiva; úsese para escenarios de capacidad, no como ROI realizado |
| Exposición técnica de tareas jurídicas a IA | **44 %** del trabajo jurídico podría exponerse a automatización, estimación de Goldman Sachs | Exposición no equivale a sustitución de abogados ni a ahorro logrado |
| TAR frente a revisión lineal | Estudios de Grossman y Cormack concluyeron que TAR puede obtener resultados comparables o mejores que revisores humanos en evaluaciones experimentales | La precisión depende de corpus, criterio de relevancia, prevalencia y control de calidad; debe medirse recall/precision del asunto |
| Exactitud de GenAI en investigación | No existe una tasa universal defendible | Debe medirse por jurisdicción, fecha, corpus y tarea: tasa de citas válidas, cobertura de autoridades y errores materiales |

**Métricas operativas recomendadas.** Antes/después, por tipo de asunto: minutos por intake; tiempo hasta conflicto despejado; tiempo de primera versión; porcentaje de campos completos; tasa de correcciones; porcentaje de citas verificadas; recall de documentos relevantes; costo externo evitado; tiempo liberado que se convierte en trabajo facturable, captación o menor plazo de entrega. Una reducción de tiempo sólo es ROI si el tiempo se monetiza, se evita gasto o aumenta la capacidad sin degradar calidad.

## 2. Comparativa internacional

### 2.1 Estados Unidos

Estados Unidos concentra el mercado de analítica litigiosa y e-discovery a escala. **Lex Machina** publica estadísticas por tribunal, juez, tipo de caso, resoluciones y duración; **Bloomberg Law Litigation Analytics** ofrece perfiles de tribunales/jueces y datos de dockets; **Westlaw Precision con CoCounsel** y **Lexis+ AI** combinan investigación con GenAI; **Relativity aiR** y **Everlaw** operan flujos de revisión e investigación documental. Esto sirve para priorizar, no para afirmar que un juez “fallará” de cierto modo: los datos de dockets no capturan necesariamente acuerdos, calidad probatoria ni hechos críticos.

En due diligence masivo, el patrón robusto es: extraer/normalizar contratos, buscar cláusulas y excepciones, clasificar riesgos, y asignar al abogado las excepciones. **Luminance**, **Kira**, **Evisort** y módulos de proveedores de e-discovery son ejemplos comerciales. El valor aparece cuando hay taxonomía de cláusulas, playbook y muestra de validación; sin ellos, el despacho sólo automatiza inconsistencia.

### 2.2 Europa: diferencias jurídicas y tecnológicas

| Jurisdicción | Adopción y software concreto | Sector público / tribunales | Límite jurídico clave | Implicación práctica |
|---|---|---|---|---|
| España | Grandes firmas y departamentos jurídicos usan gestión documental y CLM; **Bigle Legal** (CLM/automatización), **Lefebvre GenIA-L** (asistencia sobre contenidos jurídicos) y **vLex Vincent AI** (investigación) son ofertas identificables del ecosistema hispano | LexNET y expediente judicial electrónico articulan la digitalización procesal, con grados de implantación territorial distintos | RGPD, LOPDGDD y Reglamento de IA de la UE; secreto profesional y transferencia a proveedor | Separar corpus del cliente, DPA, residencia/transferencias y auditoría de respuestas |
| Italia | **Luminance**, **Docusign CLM** y automatización contractual se usan en el mercado privado; la adopción generativa está condicionada por protección de datos | Processo Civile Telematico y portales ministeriales son la base de administración digital, no una sentencia automatizada | RGPD; la decisión del Garante sobre ChatGPT de 2023 mostró la exigencia de transparencia, base jurídica y controles | No cargar expedientes identificables en un servicio sin acuerdo de tratamiento y evaluación de transferencia |
| Francia | **Doctrine**, **Predictice** y **Case Law Analytics** explotan jurisprudencia y analítica permitida; no pueden convertir la identidad de magistrados en perfil decisional | Open data de decisiones y proyectos de transformación digital judicial amplían materia prima para búsqueda | Art. 33 de la Loi n.º 2019-222 sanciona reutilizar datos de identidad de magistrados/funcionarios para evaluar, analizar o predecir sus prácticas profesionales | La analítica de decisiones es posible si no perfila al juez identificado; diseñar productos a nivel de jurisprudencia, no de persona |
| Alemania | **BRYTER** automatiza flujos; **Lawlift** automatiza contratos; **Noxtua** ofrece IA jurídica soberana/empresarial | beA, XJustiz y eAkten sostienen el intercambio y expediente electrónico; la digitalización es federal y desigual por Land | RGPD, secreto profesional (p. ej., § 203 StGB) y reglas profesionales; Reglamento de IA | Arquitectura con control de acceso, alojamiento adecuado y pruebas jurídicas en alemán |

**Aclaración francesa importante.** El artículo 33 no prohíbe toda predicción o toda IA jurídica. Prohíbe específicamente reutilizar datos de identidad de magistrados y miembros de la judicatura para evaluar, analizar, comparar o predecir sus prácticas profesionales. Por eso siguen existiendo productos de búsqueda y analítica jurisprudencial; la frontera de producto es la identificación/evaluación del decisor individual.

### 2.3 América Latina

La región tiene demanda alta —volumen procesal, informalidad documental, equipos jurídicos reducidos y presión por plazos— pero adopción desigual. Las barreras recurrentes son: baja calidad/interoperabilidad de datos judiciales, presupuesto, expedientes escaneados, conectividad, compras públicas lentas, escasez de corpus jurídicos estructurados y riesgo de enviar información confidencial a nubes fuera de la jurisdicción. Hay base sólida para automatización de intake, contratos, cobranzas, compliance y clasificación; es más débil la promesa de “predicción judicial” cuando el dato público no es completo ni comparable.

## 3. Chile: diagnóstico, regulación y oportunidades

### 3.1 Hitos normativos y de gobernanza

| Fecha | Hito | Estado e impacto para un estudio jurídico |
|---|---|---|
| 1999–2026 | Ley N.º 19.628 sobre protección de la vida privada | Marco actualmente aplicable hasta el cambio de vigencia; no autoriza por sí solo reutilización irrestricta de expedientes |
| 13-dic-2024 | Publicación de la **Ley N.º 21.719** | Reforma integral de protección de datos; crea institucionalidad y nuevo régimen de principios, derechos, responsabilidades e infracciones |
| 01-dic-2026 | Entrada en vigencia general de la Ley N.º 21.719 | Fecha de preparación crítica: inventario, contratos con encargados, seguridad, derechos y transferencias deben estar listos antes de operar |
| 2021 / actualización 2024 | Política Nacional de Inteligencia Artificial y plan de acción | Marco de política pública, no una licencia para tratar datos ni una exención del secreto profesional |
| En aplicación escalonada desde 2024 | Reglamento (UE) 2024/1689, AI Act | Relevante para firmas chilenas que ofrezcan/suministren sistemas a personas en la UE o traten datos bajo RGPD; no es una ley chilena de aplicación general |

### 3.2 Secreto profesional, custodia y evaluación de proveedor

Un modelo no es un mero procesador de texto. Si recibe nombres, RUT, correos, anexos, estrategias, declaraciones, investigaciones o contratos, participa en una cadena de tratamiento y de custodia. El abogado debe analizar además el deber de secreto profesional bajo la regulación penal, procesal y deontológica aplicable al encargo; la externalización tecnológica no debe ampliar el círculo de revelación más allá de lo necesario y autorizado.

**Lista mínima de habilitación antes de usar GenAI con información de cliente:**

1. Clasificar el dato: público, interno, confidencial, secreto profesional, dato personal, sensible o de menores.
2. Elegir la base y finalidad; aplicar minimización y seudonimización/redacción de identificadores cuando sea viable.
3. Contratar con el proveedor como encargado: instrucciones documentadas, prohibición de entrenamiento con datos del cliente, subencargados identificados, devolución/borrado, cifrado, soporte de auditoría e incidente.
4. Revisar ubicación, acceso remoto y transferencia internacional. Exigir documentación vigente del flujo de datos, no sólo la etiqueta “enterprise”.
5. Configurar SSO/MFA, roles por asunto, registros, retención, legal hold y separación de tenants.
6. Probar con un set sintético o previamente autorizado; medir citas, omisiones, privilegio y sesgo antes de producción.
7. Mantener revisión humana y registro de versión de prompt, corpus, resultado y aprobador para entregables sensibles.

### 3.3 Casos locales: evidencia y cautela

La evidencia pública chilena disponible no permite afirmar responsablemente una implantación transversal de un “motor de IA que decide” en el Poder Judicial o Ministerio Público. **PodJud/PJUD** debe tratarse ante todo como el ecosistema digital del Poder Judicial —consulta de causas, Oficina Judicial Virtual, tramitación e interoperabilidad— y no como prueba de que los tribunales deleguen decisiones a un LLM. La disponibilidad de expedientes/actuaciones digitales sí habilita automatización administrativa y analítica controlada, siempre respetando acceso, finalidad y datos reservados.

Para el mercado privado, los nombres de software sí permiten proyectos reales sin atribuir contratos no publicados: **vLex Vincent AI** para investigación con fuentes jurídicas; **Lefebvre GenIA-L** para contenido jurídico en español; **Bigle Legal** para CLM; **BRYTER** para intake/automatización; **Microsoft Azure OpenAI Service** o una plataforma equivalente con controles empresariales para casos internos; y **Docassemble** para cuestionarios de bajo coste. La contratación por una firma chilena debe verificarse caso a caso con anuncio de la propia firma o referencia contractual: una página de proveedor no demuestra que un despacho concreto esté en producción.

Esta distinción es clave para Fiscalías: no se debe presentar como hecho una adopción de IA sólo porque exista digitalización, analítica o un piloto académico. Para alegar un caso público se requiere, como mínimo, acto administrativo, licitación, comunicado institucional o informe técnico que identifique entidad, finalidad, software, periodo y salvaguardas.

### 3.4 Nichos comerciales aún subatendidos

| Nicho | Producto viable | Comprador | Indicador comercial |
|---|---|---|---|
| Cómputo de plazos y alertas verificables | Motor de reglas con calendario legal, fuente normativa y auditoría | Litigantes, cobranzas, pymes | Menos vencimientos; tiempo de preparación por causa |
| Intake laboral/consumo | Entrevista guiada, carga segura, checklist de evidencia y triage humano | Estudios boutique y sindicatos/empresas | Conversión consulta→mandato; expedientes completos |
| Contratos para pymes | Biblioteca de cláusulas chilenas, playbooks, aprobaciones y firma | Pymes, inmobiliario, procurement | Ciclo de contrato; desviaciones de cláusula |
| Privacidad y Ley 21.719 | Inventario, DSAR, registros, DPIA/EIPD, contratos de encargado | Empresas que deben adecuarse antes de dic-2026 | Proyectos de adecuación; controles aprobados |
| Compliance/investigaciones | Clasificación documental, preservación, cronología y revisión de privilegio | Empresas reguladas y firmas | Horas por GB; recall; hallazgos validados |
| Legal ops para municipios/servicios | Expediente, trazabilidad, plantillas y reportería; sin decisión automatizada | Sector público | Tiempo de respuesta y expedientes sin observación |

## 4. Firmas boutique y profesionales independientes

### 4.1 Stack proporcional y de bajo coste

| Necesidad | Opción | Coste/operación | Precaución |
|---|---|---|---|
| Formularios y entrevistas | **Docassemble** (código abierto) | Bajo coste de licencia; requiere hosting, mantenimiento y seguridad | No exponer formularios sin TLS, control de acceso y política de retención |
| Automatización de documentos | **docxtpl** / plantillas DOCX y datos estructurados | Bajo; útil para poderes, cartas y contratos simples | Versionar cláusulas y exigir revisión jurídica de la plantilla |
| Gestión de casos | **Clio Manage/Grow** o sistema equivalente | Suscripción; reduce trabajo administrativo | Confirmar disponibilidad, DPA, residencia y exportación de datos |
| Investigación asistida | **vLex Vincent AI**, **Lefebvre GenIA-L** o base jurídica contratada | Suscripción; valor si ofrece fuente/cita rastreable | Nunca confiar la cita sin abrir la fuente primaria |
| LLM interno | Modelo vía **Azure OpenAI Service** o despliegue privado de modelo abierto | Variable; enterprise/privado suele costar más que chat público | Desactivar entrenamiento por defecto, aislar datos y registrar acceso |
| CLM ligero | **Bigle Legal** o flujo de plantillas/aprobaciones | Suscripción según volumen | Definir taxonomía contractual antes de automatizar |

El software abierto reduce licencia, no la responsabilidad de operación. Un profesional solo debe preferir un flujo simple y auditable antes que un modelo local complejo sin parches, copias de seguridad, monitoreo ni capacidad para responder a incidentes.

### 4.2 Blueprint de flujo para un abogado solo

1. **Intake seguro:** formulario con aviso de confidencialidad, conflicto, consentimiento/aviso de privacidad aplicable, asunto, contraparte y documentos. Un humano aprueba antes de crear expediente.
2. **Conflictos:** búsqueda normalizada de cliente, RUT, grupo empresarial, contraparte y relacionados. Si hay posible coincidencia, detener el flujo: la IA no resuelve el conflicto.
3. **Expediente y plazos:** asignar ID, carpeta con permisos, fuente del plazo y alerta doble. El abogado valida el cálculo conforme a la norma procesal y al estado real de la notificación.
4. **Investigación:** recuperar fuentes primarias y jurisprudencia; usar GenAI sólo para mapa inicial, preguntas y síntesis con citas. Abrir cada autoridad decisiva.
5. **Borrador:** combinar cuestionario, datos aprobados y plantilla versionada. Marcar hechos no confirmados, cláusulas desviadas y campos pendientes.
6. **Control:** checklist de hechos, jurisdicción, vigencia, firmas, anexos, secreto y privilegio. Segundo revisor cuando el riesgo/valor lo justifique.
7. **Entrega y aprendizaje:** entregar versión PDF/DOCX, guardar versión aprobada, medir tiempo y correcciones; no reutilizar automáticamente material confidencial de otro cliente.

### 4.3 Modelo financiero reproducible

Supuesto conservador: profesional con tarifa efectiva de **CLP 55.000/h**, 40 horas productivas mensuales dedicadas a cuatro flujos repetibles; automatización reduce de 60 a 35 minutos cada uno (25 minutos liberados), en **80** expedientes/mes. Tiempo liberado: 80 × 25/60 = **33,3 h/mes**. Valor de capacidad teórica: 33,3 × CLP 55.000 = **CLP 1.831.500/mes**.

Si el 60 % de esa capacidad se vende o evita gasto, el beneficio realizado es **CLP 1.098.900/mes**. Con un coste mensual de CLP 250.000 (software, hosting y soporte proporcional), el beneficio neto estimado es **CLP 848.900/mes** y el ROI mensual simple es **339,6 %**: `(1.098.900 - 250.000) / 250.000 × 100`. El punto de equilibrio es `250.000 / 55.000 = 4,55` horas realizadas/mes. No incluya como beneficio horas “liberadas” que no se facturan, no evitan coste ni producen mejor servicio medible.

## 5. Plan de adopción en 90 días

| Periodo | Entregable | Criterio de salida |
|---|---|---|
| Días 1–15 | Inventario de procesos/datos; matriz de riesgos; selección de dos flujos de alto volumen y bajo riesgo | Dueño, datos, fuente legal y métrica base identificados |
| Días 16–30 | Contrato/DPA, configuración de identidad, retención y entorno de prueba | No se usa información de cliente en herramienta no aprobada |
| Días 31–60 | Piloto con corpus autorizado/sintético; plantillas, prompts y checklist | Muestra revisada; tasa de cita válida y errores documentados |
| Días 61–75 | Producción limitada y capacitación de abogados | Todo entregable tiene revisor humano y trazabilidad |
| Días 76–90 | Tablero de ROI/calidad, red-team de prompts e informe de decisión | Continuar, corregir o retirar según métrica y riesgo |

## 6. Conclusión

La ventaja competitiva sostenible no provendrá de afirmar que una IA “predice jueces” ni de subir expedientes a un chat genérico. Provendrá de convertir conocimiento jurídico en procesos: datos limpios, plantillas, reglas, fuentes verificables, revisión humana y custodia demostrable. En Chile, el mejor primer mercado es el trabajo repetible y documentable —plazos, intake, contratos, compliance de datos y legal ops— acompañado de preparación concreta para la Ley N.º 21.719. La IA generativa debe entrar después de ese perímetro de control, como copiloto auditado y no como sustituto de juicio profesional.

## Fuentes primarias y técnicas seleccionadas

1. [Ley N.º 21.719, Biblioteca del Congreso Nacional de Chile](https://www.bcn.cl/leychile/navegar?idNorma=1208040) (publicación y vigencia; comprobar siempre el texto consolidado).
2. [Ley N.º 19.628, Biblioteca del Congreso Nacional de Chile](https://www.bcn.cl/leychile/navegar?idNorma=141599).
3. [Política Nacional de Inteligencia Artificial, Ministerio de Ciencia de Chile](https://www.minciencia.gob.cl/areas/inteligencia-artificial/politica-nacional-de-inteligencia-artificial/).
4. [Thomson Reuters, *Future of Professionals Report 2024*](https://www.thomsonreuters.com/en/reports/future-of-professionals.html).
5. Maura R. Grossman y Gordon V. Cormack, [*Technology-Assisted Review in E-Discovery Can Be More Effective and More Efficient Than Exhaustive Manual Review*](https://www.ontariocourts.ca/scj/files/announcements/2011-10-12-grossman-cormack.pdf).
6. [Loi n° 2019-222, artículo 33, Légifrance](https://www.legifrance.gouv.fr/jorf/article_jo/JORFARTI000038261163).
7. [Reglamento (UE) 2024/1689 (AI Act), EUR-Lex](https://eur-lex.europa.eu/eli/reg/2024/1689/oj).
8. [Decisión del Garante italiano sobre ChatGPT, 2023](https://www.garanteprivacy.it/web/guest/home/docweb/-/docweb-display/docweb/9870847).
9. [Poder Judicial de Chile: Oficina Judicial Virtual](https://oficinajudicialvirtual.pjud.cl/).
10. [Lex Machina](https://www.lexmachina.com/), [BRYTER](https://www.bryter.com/), [Bigle Legal](https://www.biglelegal.com/), [vLex Vincent AI](https://vlex.com/products/vincent-ai/) y [Docassemble](https://docassemble.org/) (descripciones de producto; las promesas comerciales requieren validación propia).
