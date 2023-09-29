# RAMOSPROYECTO
import pandas as pd
data = pd.read_csv("/content/nacimiento.csv", encoding='ISO-8859-1', delimiter=';')
data = data.drop(['ACTIV_MADRE', 'ACTIV_PADRE', 'OCUPA_PADRE', 'OCUPA_MADRE', 'RANGO_PESO', 'TALLA', 'TIPO_PARTO', 'TIPO_ATEN'], axis=1)
data = data[data['SEXO'] < 3]
data.head()
