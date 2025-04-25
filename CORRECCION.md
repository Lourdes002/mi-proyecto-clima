# Correcciones de Código Identificadas

## Corrección 1: Falta de Enlace al Archivo CSS en el Código HTML

1.  **¿Qué mala práctica identificaste?**
    El código HTML no incluía la etiqueta `<link>` necesaria en la sección `<head>` para enlazar el archivo de estilos CSS.

2.  **¿Por qué es considerada una mala práctica?**
    Sin el enlace al archivo CSS, el navegador no puede aplicar los estilos definidos en la hoja de estilos externa. Esto resulta en una página web sin formato visual, lo que afecta negativamente la presentación y la experiencia del usuario. La separación de la estructura (HTML) de la presentación (CSS) es una práctica fundamental para la organización y mantenibilidad del código.

3.  **¿Cómo la solucionaste?**
    Se agregó la siguiente etiqueta `<link>` dentro de la sección `<head>` del archivo HTML:

    ```html
    <link rel="stylesheet" href="index.css">
    ```

4.  **¿Qué beneficios aporta tu solución?**
    Permite que el navegador aplique los estilos definidos en el archivo CSS, mejorando significativamente la apariencia visual de la página web y la experiencia del usuario. Además, al separar la presentación del contenido, se facilita la mantenibilidad y la consistencia del diseño en todo el sitio.

## Corrección 2: Comentarios insuficientes en el código HTML

1.  **¿Qué mala práctica identificaste?**
    El código HTML no incluye suficientes comentarios para describir su estructura o funcionalidad.

2.  **¿Por qué es considerada una mala práctica?**
    Porque dificulta la comprensión del proyecto para otros desarrolladores y complica el mantenimiento a largo plazo.

3.  **¿Cómo la solucionaste?**
    Agregando comentarios explicativos en las secciones del `<head>` y el `<header>` para clarificar su propósito.

4.  **¿Qué beneficios aporta tu solución?**
    Mejora la legibilidad del código, facilita el trabajo colaborativo y agiliza la futura modificación o depuración del sistema.

## Corrección 3: Falta de atributos de accesibilidad en mensajes dinámicos

1.  **¿Qué mala práctica identificaste?**
    Los elementos que muestran estados de carga y error no incluían atributos de accesibilidad.

2.  **¿Por qué es considerada una mala práctica?**
    Porque los lectores de pantalla no pueden detectar ni anunciar estos cambios, lo que afecta negativamente la experiencia de personas con discapacidades visuales.

3.  **¿Cómo la solucionaste?**
    Se agregaron atributos `role` y `aria-live` apropiados a cada sección (`status` para carga y `alert` para errores).

4.  **¿Qué beneficios aporta tu solución?**
    Mejora la accesibilidad de la aplicación, haciéndola más inclusiva y cumpliendo con buenas prácticas de desarrollo web.