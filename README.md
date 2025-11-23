# Taller1

Entrega taller 2 MINE401 - Ciencia de datos aplicada

## Autor(es):

- Juan Carlos Cepeda Valero
- José Daniel Molano Hoyos

## Objetivo

Este repositorio es la evidencia de la ejecución del Taller 2, de la materia MINE401 - Ciencia de datos aplicada, de la Universidad de los Andes en el segundo periodo del 2025. Dentro de este taller llevaremos a cabo el caso de negocio descrito en el documento ( [Taller2.pdf](Taller2.pdf) ):

> **Objetivo:** evaluar las capacidades del estudiante para aplicar técnicas de machine learning, las cuales permita descubrir insights, sugerir accionables al negocio y calcular el valor ganado.

> **Contexto del negocio:** Apoyo a una empresa de servicios inmobiliarios.

> El mercado inmobiliario Colombiano representa más del 20% del PIB del país, siendo parte integral de la economía, proporcionando empleos a través de la construcción y moviendo cantidades de dinero de órdenes significativo en compraventa de propiedades y servicios de
> alquiler.

> HabitAlpes es una startup Colombiana que está armando un portafolio de servicios de consultoría para los propietarios de vivienda y para el gobierno distrital. Entre sus diferentes proyectos se encuentran el soporte para avalúo de los precios de vivienda, la compra, remodelación y reventa de propiedades en la capital del país, consultoría y elaboración de contratos de arrendamiento, correcciones de avalúos catastrales e informes de sugerencia de reclasificación de estratos en barrios de diferentes localidades de la ciudad. Adicionalmente, la empresa busca ser efectiva al momento de ofrecer a sus clientes el portafolios de servicios más conveniente según sus necesidades.

> Es por esto por lo que HabitAlpes le ha contratado para que, usando herramientas de Machine Learning e Inteligencia de Negocios, usted participe en la implementación de uno de sus servicios. En particular, HabitAlpes quiere comenzar con la construcción de una herramienta de cálculo de precio de venta para apartamentos de la ciudad, de tal manera que sus clientes puedan ingresar la información de sus respectivos apartamentos y obtener un valor estimado sugerido que esté de acuerdo con las características y ubicación de este, y en línea con los precios de venta de propiedades similares en el sector que le permitan ser competitivos. Para comenzar, la empresa ha recopilado una muestra de la información de apartamentos en el mercado de los últimos dos meses, que servirá como su insumo para la construcción de una prueba de concepto de la herramienta.

> Adicionalmente, usted sabe que el proceso de compra requiere la inversión de 6 horas de un  perito (salario por hora: $9.500) que revise los datos y genere un precio. Con un algoritmo de Machine Learning capaz de estimar de forma precisa los montos, se estima que se reducirá el tiempo del experto a 1 hora únicamente. HabitAlpes es capaz de revisar hasta 500 apartamentos al mes. Según datos históricos, se prevé que, por cada estimación por debajo de 20 millones del valor del apartamento, el cliente solicitará un avalúo presencial, mientras que las estimaciones que sobreestiman el valor no son reportadas.

## Alcance

Con la información suministrada en el [apartamentos.csv](apartamentos.csv) y atendiendo al siguiente [diccionario de datos](DiccionarioDatos_Apartamentos.html), se llevo a cabo un analisis en 5 pasos que nos permitío generar el siguiente documento de Insigths [Insights.md](Insights.md).

Todo el proceso esta detallado paso por paso en el Jupyter Notebook [taller2.ipynb](taller2.ipynb) donde encontraran organizado en secciones caada uno de los pasos y una decripción de cierre por cada capitulo. Los pasos para ejecutar este Notebook se encuentran al final de este documento.

## Conclusiones



## Ejecutar el notebook `taller2.ipynb`

Sigue estos pasos para ejecutar el notebook de forma interactiva o automática.

1) Instrucciones para preparar el ambiente de ejecución del notebook
   Para recrear el environment desde `environment.yml`:

```bash
conda env create -f environment.yml
```

O, si prefieres usar `pip` y un virtualenv:

```bash
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
```

2) Ejecutar de forma interactiva (Jupyter Notebook o JupyterLab)

```bash
# Instala jupyter si no está disponible
conda install -n <nombre_del_env> jupyterlab -y
conda install -n jupyter jupyterlab -y
# Lanzar JupyterLab (abre en el navegador)
jupyter lab
# O usar el clásico notebook
jupyter notebook
```

3) Ejecutar el notebook por línea de comando (sin abrir UI)

Opción A — Usando `nbconvert` (incluido con Jupyter):

```bash
# Ejecuta todas las celdas y guarda el notebook ejecutado
jupyter nbconvert --to notebook --execute taller2.ipynb --output executed_Taller1.ipynb
```

Opción B — Usando `papermill` (útil para parametrizar notebooks):

```bash
# instalar papermill si no está en el environment
pip install papermill
# ejecutar y guardar salida
papermill taller2.ipynb output_taller2.ipynb
```

Notas y recomendaciones:

- Si ves errores de importación, confirma que activaste el environment correcto (`which python` y `which jupyter` deben apuntar al environment activado).
