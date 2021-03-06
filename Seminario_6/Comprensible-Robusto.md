# Comprensible y Robusto
## Criterio 3.3.1: Identificación de errores

La intención de este Criterio de Conformidad es garantizar que los usuarios sean conscientes de que se ha producido un error y puedan determinar cuál es el problema. El mensaje de error debe ser lo más específico posible.

De forma que si se detecta un error en la entrada de datos: se identifica el elemento erróneo y se describe el error mediante texto.

### Técnicas:

Existen dos situaciones a considerar:

#### Situación A: Si un formulario contiene campos para los que la información del usuario es obligatoria.

* **G83: Proporcionar descripciones de texto para identificar los campos obligatorios que no se completaron.**

El objetivo de esta técnica es notificar al usuario cuando no se ha rellenado un campo que debe completar. Cuando los usuarios no proporcionan información para los campos obligatorios del formulario, la información se proporciona en texto para permitir a los usuarios identificar qué campos se omitieron.

* **SCR18: Proporcionar validación y alerta del lado del cliente.**

El objetivo de esta técnica es validar la entrada del usuario a medida que se ingresan valores para cada campo, mediante scripts del lado del cliente. Si se encuentran errores, un cuadro de diálogo de alerta describe la naturaleza del error en el texto. Una vez que el usuario cierre el cuadro del diálogo de alerta, es útil que el script coloque el foco del teclado en el campo donde ocurrió el error.

#### Situación B: Si se requiere que la información proporcionada por el usuario esté en un formato de datos específico o de ciertos valores.

* **G85: Proporcionar una descripción de texto cuando la entrada del usuario está fuera del formato o valores requeridos.**

El objetivo de esta técnica es ayudar a corregir errores de entrada cuando no se acepta la información proporcionada por el usuario. Cuando los usuarios ingresan una entrada de datos que está validada y se detectan errores de entrada, la información sobre la naturaleza y ubicación del error de entrada se proporciona en texto para permitir a los usuarios identificar el problema.

* **ARIA18: Uso de aria-alertdialog para identificar errores.**

El propósito de esta técnica es alertar a las personas de que se ha producido un error de entrada. El uso de role = "alertdialog" crea una notificación. Esta notificación debe ser modal con las siguientes características:

  - `aria-label` o `aria-labelledby` atributo le da al alertdialog un nombre accesible.
  - `aria-describedby` proporciona una referencia al texto de la alerta.
  - El cuadro de diálogo de alerta contiene al menos un control enfocable, y el foco debe moverse a ese control cuando se abre el cuadro de diálogo de alerta.
  - El orden de las pestañas está restringido dentro del cuadro de diálogo de alerta mientras está abierto.
Cuando se cierra el cuadro de diálogo, el foco vuelve a la posición que tenía antes de que se abriera el cuadro de diálogo, si es posible.

### Tabla con ejemplos de los criterios:
![Tabla-G83](https://github.com/alu0101217741/UyA-Seminarios/blob/main/Seminario_6/img/g83.png?raw=true)
![Tabla-SRC-18-1](https://github.com/alu0101217741/UyA-Seminarios/blob/main/Seminario_6/img/src18_1.png?raw=true)
![Tabla-SRC-18-2](https://github.com/alu0101217741/UyA-Seminarios/blob/main/Seminario_6/img/src18_2.png?raw=true)
![Tabla-G85](https://github.com/alu0101217741/UyA-Seminarios/blob/main/Seminario_6/img/g85.png?raw=true)
![Tabla-Aria-18-1](https://github.com/alu0101217741/UyA-Seminarios/blob/main/Seminario_6/img/aria18_1.png?raw=true)
![Tabla-Aria-18-2](https://github.com/alu0101217741/UyA-Seminarios/blob/main/Seminario_6/img/aria18_2.png?raw=true)


