# trabajo-ciencia-datos

# datos del cliente:
SA: 1 – age: edad
VK: 2 - job : tipo de trabajo -> categorica nominal (cuantas categorias hay?, una col por categoria + top k)
SM: 3 - marital : estado civil -> categorica nominal (asignar un numero a cada categoría)
JJ: 4 – education: nivel educativo -> categorica ordinal (asignar un numero a cada categoría, ver como hacer con unknowns)
VT: 5 - default: ¿tiene crédito en mora? (creditos atrasados) -> binaria, faltantes (?) - evaluar correlacion con otras columnas (trabajo, edad) 
SA: 6 - housing: ¿tiene préstamo para vivienda? -> binaria, faltantes (?) - evaluar correlacion con otras columnas (trabajo, edad) 
VK: 7 - loan: ¿tiene préstamo personal? -> binaria, faltantes (?) - evaluar correlacion con otras columnas (trabajo, edad) 

# relacionado con el último contacto de la campaña actual:
SM: 8 - contact: tipo de contacto -> binaria (una columna 0,1)
JJ: 9 - month: último mes de contacto del año -> categorica ordinal (asignar un numero a cada categoría)
VT: 10 - day_of_week: último día de contacto de la semana -> categorica ordinal (asignar un numero a cada categoría)
SA: 11 - duration: duración último contacto, en segundos -> dividir en categorias (data binning: equal width o frequency)

# otros atributos:
VK: 12 - campaign: número de contactos realizados durante esta campaña y para este cliente -> solo evaluar si hay outliers
SM: 13 - pdays: número de días que pasaron desde la última vez que se contactó con el cliente desde una campaña anterior -> sacamos esa col (justificacion: correlacion con "previous")
JJ: 14 - previous: número de contactos realizados antes de esta campaña y para este cliente -> 
VT: 15 - poutcome: resultado de la campaña de marketing anterior -> WHAAAAAAATTTTT

# Atributos del contexto social y económico
16 - emp.var.rate: tasa de variación del empleo - indicador trimestral -> ??
17 - cons.price.idx: índice de precios al consumidor - indicador mensual -> 
18 - cons.conf.idx: índice de confianza del consumidor - indicador mensual -> 
19 - euribor3m: euribor a 3 meses - indicador diario
20 - nr.employed: número de empleados – indicador trimestral 

Variable de salida (objetivo deseado):
21 - y - ¿El cliente ha suscrito un depósito a plazo? 
