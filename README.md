# Analisis de una empresa de telecomunicaciones
## Introduccion
Empresa de telecomunicaciones *Desconnecta* con operaciones en Mexico y Colombia.

Entregar un reporte para entender como los clientes usan realmente los servicios moviles (llamadas y mensajes).

El objetivo de *Desconnecta* es identificar patrones de uso, detectar comportamientos atipicos y comprender que segmentos de clientes muestran necesidades diferenciadas, con el fin de optimizar la oferta comercial y mejorar la experiencia del usuario.

Trabajaremos con tres fuentes de datos:
- plans.csv:        Catalogo de planes con sus precios y beneficios: precio, minutos incluidos, GB incluidos, costo por extra.
- users_latam.csv:  Información de cada usuario: datos personales, plan contratado, fecha de registro, churn.
- usage.csv:        Actividad generada por los usuarios: llamadas (duracion) y mensajes (longitud).

Estos datasets se complementan para analizar el comportamiento del usuario, su consumo y cómo este se relaciona con el plan contratado, permitiendo detectar patrones de uso y churn.

Se requiere explorar, limpiar y analizar estas bases de datos para construir una vision clara, confiable y accionable sobre el comportamiento de uso de los clientes y como varia entre diferentes grupos de usuarios.

## Preguntas del negocio
- Que segmentos de clientes muestran mayor o menor uso de llamadas y mensajes?
- Que usuarios presentan valores atipicos que puedan indicar comportamientos inusuales, fraude o errores de registro?
- Como varia el uso segun la edad y el tipo de plan contratado?
- Que patrones pueden ayudar a diseñar mejores planes, optimizar la oferta y mejorar la satisfaccion del cliente?

## Objetivos del proyecto
1. Integrar y limpiar bases de datos provenientes de tres fuentes distintas.
2. Aplicar tecnicas de validacion, estandarizacion de tipos de datos y deteccion de valores inconsistentes.
3. Construir un perfil estadistico del uso (llamadas y mensajes) por cliente y por segmentos demograficos.
4. Detectar outliers y comportamientos atipicos mediante metodos estadisticos y visuales.
5. Crear segmentaciones de clientes basadas en edad, pais y comportamiento de uso.
6. Visualizar diferencias entre segmentos y extraer insights comerciales relevantes.
7. Documentar todo el proceso en un Jupyter Notebook, junto con un README reproducible y visible GitHub.

## Herramientas de la lección
- Jupyter Notebook
- Python: pandas, numpy, seaborn, matplotlib

## Plan de accion (pensamiento programatico)
Contexto del negocio
Analizaremos el negocio usando los 3 datasets (clientes, uso_real y planes) para que *Desconnecta* entienda como se comportan sus usuarios segun edad, volumen de llamadas/mensajes y nivel de consumo.
Entregaremos un analisis completo (distribuciones, outliers, segmentacion y oportunidades comerciales) acompañado de un notebook limpio y reproducible.

## Flujo general del proyecto
| Paso | Accion | Resultado para el negocio |
| :--- | :--- | :--- |
| 1. Cargar y explorar | Cargar y explorar plans, users_latam, usage | Vision clara de la estructura y tipos de columna de cada dataset |
| 2. Identificación de problemas de calidad | Contar nulos, detectar sentinels, revisar fechas fuera de rango | Lista priorizada de problemas que pueden sesgar decisiones |
| 3. Limpieza basica | Reemplazar sentinels, convertir fechas, imputar o marcar NA segun reglas | Datos consistentes y listos para analisis estadistico |
| 4. Summary statistics | Revisar las medidas clave en variables categoricas y numericas | Medidas clave (media, mediana, percentiles) que muestran el comportamiento tipico y extremo |
| 5. Visualizacion & outliers | Creacion de histogramas y boxplots | Visualizacion de sesgos, patrones de usuarios o datos atipicos |
| 6. Segmentacion | Crear segmentaciones basadas en reglas claras; visualizar proporciones con countplots | Segmentos accionables que permiten diseñar ofertas, campañas y migraciones de plan |
| 7. Insight ejecutivo | Redactar conclusiones y recomendaciones comerciales basadas en los pasos anteriores | Responder a las preguntas del negocio y proponer acciones concretas |
| 8. Publicacion | Subir el notebook + README a GitHub | Entrega reproducible para revision y ejecucion por stakeholders |
