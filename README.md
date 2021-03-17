
# Análisis de sentimientos del Ecuador 2020 COVID-19

En el año 2020, fue un año que impacto al mundo entero , con un pandemia que azoto a muchos países de nuestro, pareciera que fue sacado de una película de ciencia ficción.En el 2019, hacíamos planes o proyecciones para el 2020, pero con el coronavirus la mayoría de nuestro planes debieron cambiar, incluso a personas como estudiante que tuvieron que adaptarse ala educación en linea , a los trabajadores trabajar desde casa , y siempre tener presente un cubre boca, pero a pesar de todo lo que ha pasado en el 2020 , las personas salieron adelante, abrieron caminos donde no había antes nada , y siguieron su caminos.El ser humano es impresionante. Después de esta introducción motivacional. El presente articulo es el impacto que ha tenido el coronavirus en el Ecuador.

![https://cdn-images-1.medium.com/max/1600/1*lz6Gu-RWCwm47QjOUMwTGg.png](https://cdn-images-1.medium.com/max/1600/1*lz6Gu-RWCwm47QjOUMwTGg.png)

### Casos de coronavirus en Ecuador

Hasta el momento, el Instituto Nacional de Investigación en Salud Pública (INSPI) ha tomado **1’022.897** muestras para RT-PCR COVID-19 de las cuales **289.472 son casos confirmados con pruebas PCR.**

Este indicador, de actualización diaria, reporta el número acumulado de las muestras tomadas para la realización de la prueba RT-PCR en los laboratorios autorizados en Ecuador. Cabe indicar que puede existir más de una muestra por persona durante el proceso diagnóstico.

- **247.898** pacientes recuperados.
- **32.150** casos con alta hospitalaria.
- **11.157** personas fallecidas (confirmados COVID-19)
- **816** hospitalizados estables.
- **507** hospitalizados con pronóstico reservado.
- **679.026** casos fueron descartados.

Para analizar los sentimientos, se tuvo que recolectar datos de Twitter , para eso se utilizo una librería en **Python** llamada Twint .[Twint](https://github.com/twintproject/twint) es una herramienta avanzada de raspado de Twitter escrita en Python que permite raspar Tweets de perfiles de Twitter sin usar la API de Twitter. Twint utiliza los operadores de búsqueda de Twitter para permitirle raspar Tweets de usuarios específicos, raspar Tweets relacionados con ciertos temas, hashtags y tendencias, o clasificar información confidencial de Tweets como correos electrónicos y números de teléfono. Encuentro esto muy útil, y también puedes ser muy creativo con él. Twint también realiza consultas especiales a Twitter, lo que le permite también rastrear los seguidores de un usuario de Twitter, los tweets que le han gustado a un usuario y a quién siguen sin ninguna autenticación, API, Selenium o emulación de navegador.

Con Twint se recolecto aproximadamente 143.000 tweets desde 1 de enero hasta el 31 de enero.Para la investigación solo se utilizo 1000 tweets de forma aleatoria, el poder computacional que presento ahora no era lo suficiente para poder analizar todo el Dataset.

### **Noticias del Ecuador Relavantes**

Dentro del Dataset, habían días que tenia ma tweets en comparación a los demás, y esas fecha coinciden con estas noticias en el ecuador.

### 2020–02–29

Se confirmo el primer caso de coronavirus en el país

![https://cdn-images-1.medium.com/max/1600/1*8GAe4QVddKByqKMBedupXw.png](https://cdn-images-1.medium.com/max/1600/1*8GAe4QVddKByqKMBedupXw.png)

### 2020–01–20 — 2020–01–27

Habían rumores por varios días dentro de las redes sociales habían funcionarios públicos que supuestamente murieron con COVID19, hasta que el publicaron la falsedad del caso

![https://cdn-images-1.medium.com/max/1600/1*JAqHPv4vc4_1OtPwrpIebQ.png](https://cdn-images-1.medium.com/max/1600/1*JAqHPv4vc4_1OtPwrpIebQ.png)

### WordCloud

Antes de comenzar con los sentimientos de las personas , también se desarrollo un **WordCloud** con los tweets de los usuario , para de estar manera saber que palabras era más relevante en el Dataset

![https://cdn-images-1.medium.com/max/1600/1*DuPPypcdjB_0wM-PKeo7ow.png](https://cdn-images-1.medium.com/max/1600/1*DuPPypcdjB_0wM-PKeo7ow.png)

Word Cloud -Tweets Ecuador 2020

En la palabras mas relevantes están pandemia , casos, día, positivo , guayaquil.Guayaquil en las primeras fechas que se introdujo el coronavirus en el Ecuador , fue una de las ciudades mas afectados por el coronavirus, y había una tasa alta de contagiados y gran parte de la población se encontraba aterrorizada del caso , la mayoría que se hacían pruebas ,porque presentaba síntomas , su resultado era **positivo** al covid.

### Tópicos

Tambien se genero topicos para ver titulos fueron importantes dentro de esas fechas, para eso se LDA .**Latent Dirichlet Allocation (LDA)** es un [modelo generativo](https://es.wikipedia.org/wiki/Modelo_generativo) que permite que conjuntos de observaciones puedan ser explicados por grupos [no observados](https://es.wikipedia.org/w/index.php?title=Variable_oculta&action=edit&redlink=1) que explican porqué algunas partes de los datos son similares. Por ejemplo, si las observaciones son palabras en documentos, presupone que cada documento es una mezcla de un pequeño número de categorías (también denominados como tópicos) y la aparición de cada palabra en un documento se debe a una de las categorías a las que el documento pertenece.

![https://cdn-images-1.medium.com/max/1600/1*FFVWUCrzCdN3dkmv0J0mCg.png](https://cdn-images-1.medium.com/max/1600/1*FFVWUCrzCdN3dkmv0J0mCg.png)

### **Análisis de Sentimientos**

Como se dijo anteriormente se uso ***1000 tweets*** por cada mes, para realizar el análisis. A continuación los resultados:

![https://cdn-images-1.medium.com/max/1600/1*Zi42inQ2j7Pdygj_ArSieQ.png](https://cdn-images-1.medium.com/max/1600/1*Zi42inQ2j7Pdygj_ArSieQ.png)

### Con los datos normalizados

![https://cdn-images-1.medium.com/max/1600/1*kkpZCAScHB4JIG0QVqtXqw.png](https://cdn-images-1.medium.com/max/1600/1*kkpZCAScHB4JIG0QVqtXqw.png)

Ejemplo de Tweets NEUTRO

![https://cdn-images-1.medium.com/max/1600/1*iHLMzsSRPtMfoowjoDJSEQ.png](https://cdn-images-1.medium.com/max/1600/1*iHLMzsSRPtMfoowjoDJSEQ.png)

Ejemplo de Tweets NEGATIVO

![https://cdn-images-1.medium.com/max/1600/1*NIsMepQBqnLxJBdi6dKl0g.png](https://cdn-images-1.medium.com/max/1600/1*NIsMepQBqnLxJBdi6dKl0g.png)

Ejemplo de Tweets POSITIVO

![https://cdn-images-1.medium.com/max/1600/1*D6_Y7yj52VyxQF6knEXHMQ.png](https://cdn-images-1.medium.com/max/1600/1*D6_Y7yj52VyxQF6knEXHMQ.png)

### Conclusiones

El Ecuador fue un país que le afecto mucho la llegada de COVID , hubo muchas contagiados , a travez de los datos , los sentimientos de las personas son mas negativos es lógico es un situación que ponen en tristeza a un país, se cerraros escuelas, centro educativos , hospitales llenos , muertes , contagiados , pero poco a poco saldremos del covid 19 .La investigación se realizo solo 12000 datos o tweets aproximadamente , se puede realizar un análisis mas profundo con mas datos .Espero en el futuro realizar las prueba
