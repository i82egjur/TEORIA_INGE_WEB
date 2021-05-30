UWE diagramas y estereotipos

Dentro de las actividades que ocupa UWE, encontramos el modelado de requisitos. Dentro de este, debemos hacer de casos de uso y diagramas de actividades.
                                                        _                                                                   \ \
**Casos de uso**. Hay 2 estereotipos principales, browsing |_| (no hay modificacion persistente de datos)y processing si la hay /_/.

**Diagrama de actividades**. Se describe uno por cada caso de uso, se modelas las acciones que forman parte de estem los datos presentados y requeridos.
Para ello utilizamos los siguientes estereotipos:
![imagen](https://user-images.githubusercontent.com/55484111/120102337-c9a97a00-c14a-11eb-910e-822e7e2876f1.png)

-**<<userAction>>**: Interacciones del usuario con la web iniciando un proceso o respondiendo a un explicito requisito de informacion  
-**<<systemAction>>:** Acciones ejecutadas por el sistema 
-**<<displayAction>>:** grupos de presentacion
-**<<interactionPin>>**: datos de entrada
-**<<displayPin>>**: datos de salida                                                                   _   \
-**<<navigationAction>>**: Modelar opciones de navegacion y los elementos asociados de presentacion.  |_|->/  
  
 ## Modelado de contenido
 - Este es representado mediante un diagrama "normal" de clases.
  
  ## Modelo de navegacion
  - Resulta útil, saber como están enlazadas las páginas, para ello, partimos del modelo de contenido con sus nodos y sus enlaces y lo transformamos a un modelo
  de navegacion. 
  - Para ello, partimos del diagrama de contenido y estereotipamos con <<navigationClass>> las clases o entidades del diagrama de contenido y con <<navigationLink>> las relaciones entre estos. Después, vemos cuales de estas clases y enlaces son relevantes para la navegacion y eliminamos el resto.
  - Para navegar entre diferentes clases, en uwe se pueden utilizar menus <<menu>>.
  - Podemos listar objectos del mimso tipo usando <<index>>
  - Podemos hacer clases para buscar usando <<query>>
  - Si por ejemplo queremos crear o gestionar clases, tenemos el estereotipo <<processClass>> que unimos a los otros con <<processLink>>
  ![imagen](https://user-images.githubusercontent.com/55484111/120103423-cebcf800-c14f-11eb-8d2a-44ce7847aad0.png)

  ## Modelo de presentacion.
  - El modelo de navegacion no indica como aparece cada elemento en la web. Para ello, utilizamos el modelo de presentacion, para expresar que elemento esta ubicado en que parte de una web.
  
  ![imagen](https://user-images.githubusercontent.com/55484111/120103671-0c6e5080-c151-11eb-86ab-dd93369e6fe4.png)

  
  
  
