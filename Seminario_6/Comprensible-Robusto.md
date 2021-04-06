# Comprensible y Robusto
## Criterio 3.3.1: Identificación de errores

La intención de este Criterio de Conformidad es garantizar que los usuarios sean conscientes de que se ha producido un error y puedan determinar cuál es el problema. El mensaje de error debe ser lo más específico posible.

De forma que si se detecta un error en la entrada de datos: se identifica el elemento erróneo y se describe el error mediante texto.

### Técnicas:

Existen dos situaciones a considerar:

#### Situación A: Si un formulario contiene campos para los que la información del usuario es obligatoria.

* **G83: Proporcionar descripciones de texto para identificar los campos obligatorios que no se completaron.**

El objetivo de esta técnica es notificar al usuario cuando no se ha completado un campo que debe completar. Cuando los usuarios no proporcionan información para los campos obligatorios del formulario, la información se proporciona en texto para permitir a los usuarios identificar qué campos se omitieron.

* **SCR18: Proporcionar validación y alerta del lado del cliente.**

El objetivo de esta técnica es validar la entrada del usuario a medida que se ingresan valores para cada campo, mediante scripts del lado del cliente. Si se encuentran errores, un cuadro de diálogo de alerta describe la naturaleza del error en el texto. Una vez que el usuario cierre el cuadro del diálogo de alerta, es útil que el script coloque el foco del teclado en el campo donde ocurrió el error.


