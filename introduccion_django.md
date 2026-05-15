1. ¿Qué es Django?
    -¿Qué tipo de framework es?
    Es un framework web de alto nivel, de código abierto y escrito en Python. viene con casi todo lo necesario para desarrollar una aplicación funcional desde el primer momento.

    -¿Qué tipo de aplicaciones permite construir?
    Permite construir prácticamente cualquier cosa: desde blogs sencillos y sistemas de gestión de contenido (CMS) hasta redes sociales complejas (como Instagram), plataformas de streaming o herramientas de análisis de datos científicos.
    
    -Menciona al menos tres ventajas de usar Django sobre trabajar con Python puro para desarrollo web.
    Velocidad de desarrollo: Django automatiza tareas repetitivas, permitiéndote pasar del concepto al lanzamiento en mucho menos tiempo.
    Seguridad integrada: Protege automáticamente contra ataques comunes como SQL Injection, Cross-Site Scripting (XSS) y CSRF.Escalabilidad: Está diseñado para manejar volúmenes masivos de tráfico y datos de manera eficiente.
    
    2. Entornos virtuales en Python
    -¿Qué es un entorno virtual en Python y para qué sirve?
    Un entorno virtual es un espacio aislado dentro de tu computadora donde puedes instalar versiones específicas de librerías para un proyecto sin afectar a los demás proyectos ni al sistema operativo.
    
    -¿Qué ventajas tiene crear un entorno virtual para un proyecto Django?
    Evita conflictos de versiones en la misma máquina sin que choquen entre sí. Además, facilita compartir el proyecto con otros desarrolladores asegurando que todos usen las mismas dependencias.
    
    -Explica en tus palabras qué hace el siguiente comando (no es necesario ejecutarlo):python -m venv env.
    Este comando le dice a Python que ejecute el módulo encargado de crear entornos virtuales (venv) y que cree una carpeta llamada env donde se guardará toda la copia aislada de Python y las librerías que instales.
    
    3. Estructura y diseño de Django.
    -¿Qué es el patrón MVC y cómo se aplica en Django (MTV)?
    Django utiliza el patrón MTV (Model-Template-View), que es una adaptación del clásico MVC.
    Aunque Django se basa en el concepto tradicional de MVC (Modelo-Vista-Controlador), los creadores del framework decidieron usar el nombre MTV (Modelo-Template-Vista) porque consideran que el "Controlador" ya está integrado en el propio framework (el sistema de enrutamiento de URLs).
    
   -Completa esta tabla comparativa:
   ¿Por qué Django es diferente?
    En el MVC tradicional, la View es lo que el usuario ve y el Controller es la lógica. En Django:

    El framework mismo (el motor de URLs) actúa como el controlador inicial.

    La View de Django se encarga de la lógica (lo que haría un controlador).

    El Template de Django se encarga de la visualización (lo que haría una vista).

    ### Tabla Comparativa: Arquitectura Django

| Concepto Tradicional (MVC) | Equivalente Django (MTV) | Archivo Clave | Responsabilidad |

| **Model**                  | **Model**                | `models.py` | Definición de tablas y persistencia de datos. |
| **View**                   | **Template**             | `*.html`    | Interfaz de usuario y diseño visual. |
| **Controller**             | **View**                 | `views.py`  | El "puente" que procesa la lógica y une el modelo con la plantilla. |
   
    
    -¿Qué es el enrutador de Django y qué papel cumple en una aplicación web?
    Es el archivo urls.py. Su papel es el de un "recepcionista": recibe la dirección (URL) que el usuario escribe en el navegador y decide a qué View (función de Python) debe enviarla para procesar la petición.
    
    4. Principios del desarrollo con Django
    -• ¿Qué significa el principio DRY ("Don't Repeat Yourself") y cómo lo aplica Django?
    Significa evitar la duplicación de información. Django lo aplica permitiendo reutilizar código mediante la herencia de templates, el uso de formularios automáticos y la definición de modelos en un solo lugar. Si cambias algo una vez, se refleja en todo el sistema.

    -¿Qué significa que Django tenga una “estructura flexible y minimalista”?
    Estructura flexible y minimalista:Se refiere a que, aunque Django te da una estructura base, tú tienes el control total para organizar tus aplicaciones. Es minimalista porque no te obliga a usar librerías externas pesadas si no las necesitas; puedes empezar con lo básico e ir escalando.
    
    -• ¿Qué son los Templates en Django y qué rol cumplen en la renderización de contenido?
    Son archivos de texto (generalmente HTML) que definen la estructura de la página web. Su rol es la renderización de contenido: permiten insertar datos dinámicos provenientes de la base de datos dentro del código HTML utilizando un lenguaje de etiquetas especial.