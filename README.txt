# Customer_demand_prediction

AXYZ es una empresa chilena especializada en arquitectura y regularización de propiedades, ofreciendo
servicios que aseguran el cumplimiento de normativas legales en proyectos de construcción
y reformas. Analizaremos como aportar soluciones basadas en análisis de datos y machine learning
para abordar desafíos comunes en este sector.

Proyecto: Predicción de la demanda de clientes o mejorar la captación

Objetivo del proyecto: Predecir la cantidad de clientes e ingresos futuros para mejorar la planificación.

Este proyecto busca Predecir si un cliente contratará o no un servicio utilizando datos
históricos de la empresa.

Preguntas de Hipótesis: ¿Qué tipo de clientes están más interesados en contratar un servicio?
Quienes son? Donde se encuentran? Que servicios contratan? como llegan? a través de que canales
contactan?

0.2 Descripción de los datos

El dataset contiene las siguientes columnas clave para nuestro modelo:
- `fecha_registro` — Año en que el cliente se registró;
- `estado` — Si - el cliente contrató o no contrató el servicio (ideal para un modelo de clasificación);
- `nombre_completo` — Nombre completo del cliente
- `genero` — Información - sobre el perfil del cliente;
- `canal_contacto` — Cómo llegó - el cliente (Embajador, Google, Teléfono, etc.);
- `comuna` — Ubicación del cliente;
- `región` — Ubicación del cliente;
- `telefono` — Teléfono del cliente;
- `email` — email del cliente;
- `destino` — servicio solicitado (ej. Regularización de viviendas).

0.2.1 Condiciones:

#Convertir la columna objetivo “Estado” en formato numérico:

Contratado → 1 No Contratado → 0
Característica objetivo: la columna ‘Estado’

Métrica principal: AUC-ROC.
Métrica adicional: exactitud. 1

Criterios de evaluación:
• AUC-ROC < 0.75 — 0 SP
• 0.75   AUC-ROC < 0.81 — 4 SP
• 0.81   AUC-ROC < 0.85 — 4.5 SP
• 0.85   AUC-ROC < 0.87 — 5 SP
• 0.87   AUC-ROC < 0.88 — 5.5 SP
• AUC-ROC   0.88 — 6 SP