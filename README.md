# Estimación de Niveles de Obesidad en América Latina: Un Enfoque de Aprendizaje No Supervisado


  
# **:books: Acerca de**

La obesidad es un problema de salud pública creciente en varios países de América Latina, donde factores como los hábitos alimenticios, el nivel de actividad física y los antecedentes familiares tienen un papel relevante. La detección temprana, el monitoreo constante y la implementación de acciones efectivas para la prevención y reducción de la obesidad son claves para mejorar la calidad de vida de las personas.
Este proyecto aborda este desafío mediante la incorporación de técnicas de aprendizaje no supervisado, para desarrollar modelos que identifiquen patrones de riesgo y sean insumo para proporcionar recomendaciones personalizadas, apoyando los esfuerzos de prevención y tratamiento de obesidad en países de América Latina como México, Perú y Colombia.



# **:open_file_folder: Investigación**

Sobre este tema hay varios estudios y aplicaciones, resaltamos dos de interés aplicadas en América Latina

<details>
  <summary>Aplicación de técnicas de clustering para la detección de obesidad en datos de salud en Colombia [3]</summary>
  <p>Este estudio aplica técnicas de clustering, como K-means y clustering jerárquico, para analizar datos de salud en Colombia y clasificar a los individuos en diferentes niveles de obesidad. El enfoque permite una mejor comprensión de los patrones de obesidad en la población colombiana y facilita la formulación de estrategias de intervención localizadas.</p>
</details>

<details>
  <summary>Predicción de riesgos en salud, para personas con obesidad empleando técnicas de aprendizaje de máquinas [4]</summary>
  <p>Este artículo investiga el uso de técnicas de aprendizaje no supervisado, incluyendo PCA y clustering, para analizar datos de obesidad en una muestra representativa de la población colombiana. El estudio muestra cómo estas técnicas pueden mejorar la identificación de patrones y tendencias relacionadas con la obesidad.</p>
</details>


# **:bar_chart: Sobre los datos**

Para el desarrollo del proyecto se utiliza un conjunto de datos que combina datos reales y datos sintéticos que contribuye a la precisión del modelo, se utilizan 77% datos generados y 23% de los datos recolectados directamente de usuarios a través de una encuesta en una plataforma web.

Los datos utilizados en este análisis provienen del dataset titulado "Estimation of Obesity Levels Based on Eating Habits and Physical Condition", disponible en el UCI Machine Learning Repository. Este conjunto de datos contiene información sobre los niveles de obesidad de individuos en México, Perú y Colombia, basado en sus hábitos alimenticios y condiciones físicas. 
El dataset consta de 2111 registros y 17 variables, de las cuales 16 son características del individuo que lo clasifican en un nivel de obesidad registrado en la variable “NObeyesdad” A continuación se describen las variables:

<details>
  <summary>Variables Categóricas</summary>
  <p>Gender: Género del individuo (Masculino/Femenino).
    
family_history_with_overweight: Indica si el individuo tiene antecedentes familiares de sobrepeso (Sí/No).

FAVC: Indica si el individuo consume alimentos altos en calorías frecuentemente (Sí/No).

CAEC: Indica si el individuo consume alimentos entre comidas (No/Sí).

SMOKE: Indica si el individuo fuma (Sí/No).

SCC: Indica si el individuo monitorea las calorías que consume diariamente (Sí/No).

CALC: Frecuencia con la que el individuo consume alcohol (Nunca/Rara vez/Frecuentemente/Siempre).

MTRANS: Medio de transporte que el individuo utiliza normalmente (Automóvil/Moto/Bicicleta/A pie/Transporte público).

NObeyesdad: Nivel de obesidad, categorizado en 'Insufficient_Weight', 'Normal_Weight', 'Overweight_Level_I', 'Overweight_Level_II', 'Obesity_Type_I', 'Obesity_Type_II' y 'Obesity_Type_III'.
</p>
</details>

<details>
  <summary>Variables Continuas</summary>
  <p>Age: Edad del individuo (en años).
    
Height: Altura del individuo (en metros).

Weight: Peso del individuo (en kilogramos).

NCP: Número de comidas principales que el individuo consume diariamente.

CH2O: Cantidad de agua que el individuo consume diariamente (en litros).

FAF: Frecuencia de actividad física del individuo (en días por semana).

TUE: Tiempo de uso de dispositivos tecnológicos por día (en horas).</p>
</details>



# **:hammer_and_pick: Desarrollo**

Para este desarrollo se propone utilizar algoritmos de clustering para realizar la segmentación de las personas en diferentes categorías de obesidad.

<details>
  <summary>K-means</summary>
  <p>Puede ser un método adecuado en este contexto por su simplicidad y eficiencia computacional, así como su capacidad de manejar datos categóricos y continuos. Con este algoritmo se pueden clasificar a las personas en diferentes niveles de riesgo de obesidad basándose en sus hábitos alimenticios, actividad física, y otras variables de salud.</p>
</details>

<details>
  <summary>Clustering Jerárquico</summary>
  <p>Con este algoritmo se puede construir una jerarquía de clusters para visualizar cómo los individuos se agrupan progresivamente a diferentes niveles, proporcionando una comprensión más detallada de la estructura de los datos. Adicionalmente, puede ser útil para identificar factores críticos que contribuyen a la obesidad.</p>
</details>

<details>
  <summary>DBSCAN (Density-Based Spatial Clustering of Applications with Noise)</summary>
  <p>La capacidad de este algoritmo para identificar clusters irregulares y detectar ruido puede ser valiosa en este desarrollo, ya que puede diferenciar grupos de personas en riesgo de obesidad de forma más clara y así mismo identificar los individuos que no encajan claramente con los patrones. Adicionalemnte, al utilizar datos reales y sintéticos es clave contar con un buen manejo de outliers o ruido en los datos.</p>
</details>




# **:page_with_curl: Referencias**

1. Estimation of Obesity Levels Based On Eating Habits and Physical Condition . (2019). UCI Machine Learning Repository. https://doi.org/10.24432/C5H31Z.
2. Organización Mundial de la Salud. (2023). Obesidad y sobrepeso.  https://www.who.int/es/news-room/fact-sheets/detail/obesity-and-overweight
3. Organización Panamericana de la Salud. (2022). Obesidad: una preocupación de salud pública. Prevención de la obesidad - OPS/OMS | Organización Panamericana de la Salud (paho.org)
4. Gómez, M. A., & Henao, H. (2020). Aplicación de técnicas de clustering para la detección de obesidad en datos de salud en Colombia. Revista Colombiana de Estadística, 43(2), 209-225. Las variables más influyentes en la obesidad: un análisis desde la minería de datos (scielo.cl)
5. Agamez Julio, Wilmer Jesús. (2022). Predicción de riesgos en salud, para personas con obesidad empleando técnicas de aprendizaje de máquinas. Predicción de riesgos en salud, para personas con obesidad empleando técnicas de aprendizaje de maquinas (unal.edu.co)

