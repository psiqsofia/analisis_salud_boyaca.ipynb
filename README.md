***Modelo predictivo de especialidades nédicas en un hospital de Puerto Boyacá***

Este proyecto desarrolla un modelo predictivo basado en técnicas de Machine Learning (regresión logística, random forest, gradient boosting, entre otros) para analizar y predecir patrones en las atenciones médicas de un Hospital público en el municipio de Puerto Boyacá. Se identifican las especialidades más demandadas y se exploran patrones por género, rango etario y entidad del usuario. A partir del análisis exploratorio y predictivo, se desarrollaron modelos de machine learning para clasificar y predecir las especialidades médicas más probables de atención según las características del paciente.

📊 **Objetivos**

Analizar la distribución de pacientes teniendo en cuenta el boletín del Plan de Desarrollo de Puerto Boyacá (https://puertoboyaca-boyaca.gov.co/MiMunicipio/ProgramadeGobierno/1_PDM_PPD-2024-2027.pdf). 

Identificar tendencias en las principales atenciones médicas según especialidad, edad y género.

Aplicar modelos predictivos para estimar la especialidad médica más probable.

🔍 Metodología

- Limpieza y exploración de datos (EDA), normalizando columnas, nombres y eliminando los datos nulos. Debido a la baja demanda de algunas especialidades, se optó por unificar citas de imagenologías (RX, tomografías...) y de salud visual (oftalmología y optometría)
- Se analizaron tendencias en las citas del Hospital José Cayetano Vasquez, separando por rangos de edad, sexo, entidad de afiliación del paciente.
- Se estudiaron las tres áreas prioritarias del boletín de salud pública: enfermedades cardiovasculares, musculoesqueléticas y de salud mental, mediante las atenciones de las especialidades que pueden atender estos casos. 

**Modelado predictivo:**
Se aplicaron y compararon varios modelos, con fines de estudio y para evaluar cuáles son los mejores métodos para este tipo de datasets:
- Regresión Logística
- Bosques Aleatorios (Random Forest)
- Gradient Boosting
- K-Nearest Neighbors (KNN)
- Naive Bayes
- Support Vector Machines (SVM)
  Evaluación del desempeño:
Los modelos se compararon usando Accuracy y F1-score.
Los mejores resultados se obtuvieron con **Random Forest y Gradient Boosting, con una precisión promedio del 46%.**

💡 Conclusiones

Las especialidades con mayor demanda fueron medicina general (45% del total de atenciones), odontología, PYP y medicina interna ; las que tienen menos atenciones son trabajo social, citas postquirúrgicas y de monitoreo.
Se evidenciaron diferencias significativas por género y rango de edad: las mujeres asisten en una medida muy superior a las distintas especialidades médicas, lo que plantea interrogantes sobre el autocuidado de la población másculina, teniendo en cuenta que son ellos quienes presentan más muertes violentas y accidentales en el departamento.
Los modelos predictivos permitieron identificar patrones útiles para orientar la planificación de servicios médicos, sin embargo el alcance es limitado debido a que el análisis corresponde únicamente al año 2022.

🩺 Conclusiones en relación con Políticas Públicas:

El análisis evidenció que las citas de Medicina General concentran el 45 % del total de atenciones, reflejando un** modelo asistencial reactivo más que preventivo**. La especialidad PYP predomina solo en la niñez y desaparece en la adultez, lo que sugiere la necesidad de fortalecer estrategias de promoción y detección temprana.

Se observó una marcada brecha de género en el acceso a servicios médicos: **los hombres asisten hasta un 60 % menos** que las mujeres a partir de la adolescencia. Este patrón, asociado a normas culturales de masculinidad, indica la importancia de diseñar políticas de salud con enfoque diferencial de género que promuevan la atención preventiva masculina.

Al agrupar las especialidades en tres bloques estratégicos (cardiovascular–metabólico, musculoesquelético y salud mental), se identificaron patrones de uso diferenciados por edad y sexo, relevantes para la planificación territorial en salud; por ejemplo amplia brecha de género en atenciones en salud mental (**366 %** más consultas femeninas).

Finalmente, los modelos predictivos desarrollados (Random Forest y Gradient Boosting) alcanzaron un 46 % de exactitud, demostrando el potencial del aprendizaje automático para anticipar la demanda de servicios médicos y optimizar la asignación de recursos en el sistema de salud.

⚙️ Tecnologías utilizadas

-Python 🐍

-Pandas, NumPy

-Matplotlib, Seaborn

-Scikit-learn, Imbalanced-learn

🚀 Ejecución del proyecto

Clona este repositorio

git clone https://github.com/tuusuario/tu-repo.git
cd tu-repo

Instala las dependencias
pip install -r requirements.txt

Abre el notebook
jupyter notebook proyecto_especialidades.ipynb

🧠 Autora

Juliana Sofía Gómez H.
📍 Psicóloga - Científica de Datos
💼 Interés en proyectos de salud pública, People Analytics y Business Intelligence

📈 Resultados Destacados

| Modelo              | Accuracy | F1-Macro |
| ------------------- | -------- | -------- |
| Logistic Regression | 0.406    | 0.411    |
| Random Forest       | 0.458    | 0.463    |
| Gradient Boosting   | 0.460    | 0.466    |
| SVM                 | 0.428    | 0.430    |

🏷️ Etiquetas

#MachineLearning #SaludPública #Boyacá #Python #DataScience
