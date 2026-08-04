Modelo  de  clasificación  para 
predecir la mora bancaria. 
Introducción 
Características y motivación del proyecto 
Este  proyecto  desarrolla  un  modelo  de  clasificación  aplicado  al  área  de  gestión  de  riesgo 
crediticio,  abordando  un  problema  de  aprendizaje  supervisado  orientado  a  estimar  la 
probabilidad de mora de nuevos clientes. 
La  mora  en  el  cumplimiento  de  obligaciones  crediticias  constituye  un  fenómeno  recurrente 
dentro  de  la  actividad  financiera  y,  bajo  determinados  niveles,  forma  parte  del 
funcionamiento  normal  del  sistema  bancario.  Sin  embargo,  en  contextos  de  recesión 
económica,  inflación  elevada  y  deterioro  del  poder  adquisitivo,  el  incremento  sostenido  de  la 
morosidad  puede  afectar  negativamente  la  rentabilidad,  la  liquidez  y  las  expectativas  de  los 
inversores sobre las entidades financieras. 
En  los  últimos  años,  distintas  entidades  financieras  y  fintechs  registraron  incrementos 
significativos  en  sus  niveles  de  mora,  especialmente  en  segmentos  de  consumo  y  crédito 
personal.  Estos  procesos  evidencian  las  dificultades  de  los  sistemas  tradicionales  de 
evaluación  crediticia  para  anticipar  cambios  bruscos  en  el  comportamiento  de  pago  de  los 
clientes en contextos de elevada incertidumbre macroeconómica. 
Habitualmente,  las  entidades  financieras  evalúan  el  riesgo  crediticio  mediante  instrumentos 
como  el  score  bancario  y  la  clasificación  financiera  del  cliente,  los  cuales  se  basan 
principalmente  en  el  historial  financiero  y  el  comportamiento  previo  de  pago.  Si  bien  estos 
mecanismos  resultan  eficaces  en  contextos  relativamente  estables,  pueden  presentar 
limitaciones  para  capturar  cambios  recientes  en  las  condiciones  económicas  y  financieras 
de los individuos. 
En  este  contexto,  el  área  de  riesgo  crediticio  enfrenta  un  desafío  central:  mejorar  la 
capacidad  de  identificar  clientes  con  elevada  probabilidad  de  incumplimiento  sin  restringir 
excesivamente  el  otorgamiento  de  crédito.  A  partir  de  esta  problemática,  el  presente 
proyecto  propone  desarrollar  un  modelo  de  clasificación  basado  en  técnicas  de  Machine 
Learning,  capaz  de  segmentar  clientes  según  su  probabilidad  estimada  de  incurrir  en  mora  y 
contribuir a una toma de decisiones crediticias más eficiente. 
Puntos críticos del negocio crediticio: 
Masividad de Clientes morosos: 
●  Se  otorgan  créditos  masivos  de  montos  relativamente  bajos  que  no  tienen  retorno  en 
los plazos esperados. 
Créditos no pagados: 
●  Un  porcentaje  de  los  clientes  morosos  no  pagan  sus  créditos  y  la  probabilidad  de 
recuperación es baja. 
Objetivo General 
El  objetivo  de  este  proyecto  es  crear  un  modelo  de  clasificación  que  prediga  qué  clientes 
son  candidatos  a  incurrir  en  mora  y,  a  partir  de  ello,  clasificar  el  riesgo  de  asignación  de 
nuevos créditos. 
Objetivos Específicos: 
●  Describir  las  principales  variables  financieras  y  sociodemográficas  de  los  receptores 
de crédito. 
●  Analizar  cómo  se  relaciona  la  mora  con  el  pérfil  financiero  y  sociodemográfico  del 
cliente. 
●  Crear  un  modelo  de  clasificación  utilizando  random  forest  que  prediga  la 
probabilidad de mora. 
●  Segmentar a los clientes según el riesgo a incurrir en mora. 
Perfil del cliente beneficiario: 
La solución de este proyecto va dirigida a distintas áreas de una compañía: 
Área de riesgo crediticio  →  Mejorar políticas de aprobación de créditos. 
Área comercial  → Ofrecer productos adecuados al riesgo crediticio del cliente. 
Área de cobranzas  → Campañas preventivas y renegociación crediticia. 
Adquisición de datos: 
Se  utiliza  un  dataset  de  datos  crediticios  de  Perú  descargado  de  la  plataforma  Kaggle.  El 
dataset  cuenta  con  una  dimensión  de  8399  filas  y  14  columnas.  Tras  la  limpieza  de  datos, 
transformación  de  valores  y  creación  de  nueva  variables  el  dataset  adquiere  una  dimensión 
de 6074 filas y 29 columnas. 
La  razon  por  las  cuales  se  selecciona  este  dataset  radica  principalmente  en  que  se 
encuentra  disponible  para  descargar  y  cuenta  con  más  de  70%  de  clientes  con  mora,  lo  que 
lo hace un dataset significativo para el análisis de “mora masiva”. 
No  obstante,  la  falta  de  información  acerca  del  origen  de  los  datos  alerta  sobre  la  fiabilidad 
del  mismo.  El  elevado  porcentaje  de  morosos  y  otras  inconsistencias  detectadas  advierten 
 de  elevadas  probabilidades  de  que  se  trate  de  un  dataset  sintético.  A  pesar  de  estas 
 incosistencias,  como  el  objetivo  de  este  proyecto  es  formativo,  intentaremos  subsanar  los 
 déficits del dataset con el conocimiento y las habilidades aprendidas. 
