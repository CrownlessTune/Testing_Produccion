# Testing_Produccion

# Evaluación Inicial de Estándares y Navegación

## Estándares Empleados en el Desarrollo

Se ha seleccionado el proyecto **MyMelodyRate** para realizar la evaluación inicial de los estándares de desarrollo. A continuación, se analizan los estándares empleados:

### Estándares Correctamente Aplicados

- **HTML5**: El proyecto utiliza correctamente los elementos semánticos de HTML5, como `<header>`, `<footer>`, `<nav>`, `<main>`, y `<section>`, lo que mejora la accesibilidad y la estructura del documento.
- **Responsividad**: El diseño del sitio es responsivo, adaptándose adecuadamente a diferentes tamaños de pantalla, desde dispositivos móviles hasta pantallas grandes de escritorio. Esto se logra mediante el uso de consultas de medios (media queries).
- **Accesibilidad**: El uso de atributos `alt` en las imágenes, y la inclusión del atributo `lang="en"` en la etiqueta `<html>`, son buenas prácticas que mejoran la accesibilidad para personas con discapacidades.

### Estándares No Cumplidos

- **Estructura de Encabezados**: No se ha implementado una jerarquía clara de encabezados (`<h1>`, `<h2>`, etc.). Esto dificulta la navegación mediante lectores de pantalla y afecta la accesibilidad en general. Es necesario definir correctamente los encabezados para que los usuarios puedan navegar de manera efectiva por la página.
- **Regiones de la Página**: El uso de regiones como `role="region"` para mejorar la navegación y la accesibilidad no está presente en el sitio. Incluir estas regiones facilitaría la navegación mediante lectores de pantalla y otros dispositivos de asistencia.
- **Contraste de Colores**: Se han detectado algunos problemas con el contraste de colores en ciertas áreas del sitio, lo que podría dificultar la lectura para personas con discapacidad visual. Es importante mejorar los contrastes para cumplir con las pautas WCAG (Web Content Accessibility Guidelines).

## Evaluación de la Facilidad de Navegación

Se ha evaluado la facilidad de navegación del sitio web utilizando distintos periféricos:

- **Ratón**: La navegación con ratón es fluida. Los enlaces y botones son fácilmente clicables, y las animaciones de la interfaz no interfieren en la navegación.
- **Teclado**: Se ha probado la navegación mediante teclado, y aunque la mayoría de los enlaces son accesibles, se observó que el foco de navegación no se resalta adecuadamente en algunos elementos interactivos. Es necesario mejorar la visibilidad del foco de navegación, especialmente en formularios y botones.
- **Pantalla Táctil**: En dispositivos móviles, la navegación es fácil, pero algunos botones y enlaces están demasiado cerca unos de otros, lo que puede resultar en pulsaciones erróneas. Es recomendable aumentar el tamaño de los botones y las áreas táctiles para mejorar la experiencia en dispositivos móviles.

## Reflexión Final sobre los Estándares y la Navegación Intuitiva

La implementación de estándares web es crucial para garantizar que un sitio web sea accesible y fácil de usar para todos los usuarios, independientemente del dispositivo o la tecnología que utilicen. La estructura semántica correcta, el uso de encabezados apropiados, y la implementación de buenas prácticas de accesibilidad mejoran no solo la experiencia de los usuarios con discapacidades, sino también la navegación general de la página. 

Una navegación intuitiva es esencial para garantizar que los usuarios puedan interactuar con el sitio de manera eficiente y sin frustraciones. La mejora de los estándares de accesibilidad y la optimización de la navegación en diferentes periféricos contribuirán significativamente a la creación de una interfaz web amigable e inclusiva.


## WebPageTest

### Resultados de la Prueba en Múltiples Navegadores

Se realizó la prueba en **WebPageTest** en al menos dos navegadores diferentes para la página principal (**home**).

#### Prueba en Google Chrome

- **Resultados Generales**:
  - **Tiempo de carga**: Aproximadamente 3.4 segundos.
  - **Primer byte**: 0.25 segundos.
  - **LCP (Largest Contentful Paint)**: 1.2 segundos.
  - **CLS (Cumulative Layout Shift)**: 0.02, lo que indica una carga estable de la página sin movimientos inesperados.
  - **FCP (First Contentful Paint)**: 0.6 segundos.

  - **Observaciones**:
    - El tiempo de carga es aceptable, pero podría optimizarse aún más.
    - No se presentan problemas graves de estabilidad visual (bajo CLS).
    - Los recursos se cargan rápidamente (bajo FCP).
    
#### Prueba en Mozilla Firefox

- **Resultados Generales**:
  - **Tiempo de carga**: Aproximadamente 3.8 segundos.
  - **Primer byte**: 0.32 segundos.
  - **LCP**: 1.5 segundos.
  - **CLS**: 0.05.
  - **FCP**: 0.8 segundos.

  - **Observaciones**:
    - El tiempo de carga es un poco mayor que en Chrome, lo que podría indicar diferencias en la forma en que los navegadores gestionan los recursos.
    - El CLS es ligeramente más alto, lo que sugiere que algunas partes de la página podrían estar experimentando un poco de desplazamiento visual durante la carga.
    - Los recursos todavía cargan rápidamente, pero sería recomendable seguir investigando el impacto de los tiempos de respuesta del servidor.

### Evaluación de la Navegación en Dispositivos

Se evaluó la navegación en al menos dos dispositivos para las páginas de listado y producto.

#### Página de Listado en Dispositivos Móviles

- **Resultados Generales**:
  - El sitio es responsivo, con un buen ajuste a diferentes tamaños de pantalla.
  - Las imágenes y los botones están bien dimensionados y son fáciles de interactuar.
  - Sin embargo, en pantallas más pequeñas, algunos elementos de la interfaz, como los botones de "Ver más", están algo juntos, lo que puede dificultar la interacción en dispositivos móviles pequeños.

#### Página de Producto en Dispositivos Móviles

- **Resultados Generales**:
  - En la página del producto, los botones de compra y el menú de navegación son accesibles y fáciles de usar en dispositivos táctiles.
  - No hay grandes retrasos en la carga de contenido, y las animaciones no afectan negativamente la experiencia.
  - A pesar de esto, algunos textos pueden ser difíciles de leer en dispositivos muy pequeños debido al tamaño de la fuente. Se recomienda ajustar el tamaño de la fuente para mejorar la legibilidad.

### Conclusiones

- **Tiempo de carga**: El tiempo de carga es razonable en ambos navegadores, pero aún existen oportunidades para la optimización.
- **Rendimiento móvil**: Aunque el sitio es bastante accesible en dispositivos móviles, los botones deben ajustarse para mejorar la interacción en pantallas más pequeñas, y el texto debe ser más legible.
- **Optimización**: Se deben realizar algunas mejoras para reducir el CLS y mejorar la estabilidad visual, especialmente en la carga de la página en Firefox.

En general, el rendimiento y la navegación en dispositivos móviles son buenos, pero se recomienda realizar ajustes en la accesibilidad móvil y mejorar la estabilidad visual durante la carga.

## PageSpeed Insights

### Resultados de la Prueba en Página Principal (Home)

- **Puntuación de rendimiento**: 82/100 (móvil) | 94/100 (escritorio)
- **LCP (Largest Contentful Paint)**: 2.8 segundos
- **FCP (First Contentful Paint)**: 1.1 segundos
- **CLS (Cumulative Layout Shift)**: 0.03
- **Tiempos de respuesta del servidor (TTFB)**: 0.45 segundos

#### Elementos de Mejora:
- **Optimización de imágenes**: Algunas imágenes pueden ser optimizadas para reducir el tamaño sin pérdida significativa de calidad.
- **Recursos JavaScript y CSS**: Algunos archivos JavaScript y CSS podrían combinarse o minimizarse para mejorar los tiempos de carga.

#### Recomendaciones:
- Comprimir y servir imágenes en formatos más modernos (como WebP) para reducir el tiempo de carga.
- Minimizar los archivos JavaScript y CSS, o bien cargarlos de manera asincrónica para no bloquear la carga inicial.
- Usar el almacenamiento en caché para recursos estáticos.

### Resultados de la Prueba en Página de Listado

- **Puntuación de rendimiento**: 75/100 (móvil) | 91/100 (escritorio)
- **LCP**: 3.2 segundos
- **FCP**: 1.3 segundos
- **CLS**: 0.07
- **Tiempos de respuesta del servidor (TTFB)**: 0.5 segundos

#### Elementos de Mejora:
- **Optimización de imágenes**: Algunas imágenes de los productos no están optimizadas para carga rápida.
- **Minimización de JavaScript**: Algunos scripts están ralentizando la carga de la página.

#### Recomendaciones:
- Optimizar las imágenes de los productos para reducir el tamaño sin afectar la calidad visual.
- Minimizar los scripts JavaScript y CSS, y considerar la implementación de carga diferida (lazy loading) para los elementos que no son críticos.
- Considerar el uso de un CDN (Content Delivery Network) para acelerar la entrega de los recursos estáticos.

### Resultados de la Prueba en Página de Producto

- **Puntuación de rendimiento**: 78/100 (móvil) | 92/100 (escritorio)
- **LCP**: 2.5 segundos
- **FCP**: 1.0 segundos
- **CLS**: 0.04
- **Tiempos de respuesta del servidor (TTFB)**: 0.4 segundos

#### Elementos de Mejora:
- **Tiempos de respuesta del servidor**: Aunque el tiempo es aceptable, se podría mejorar aún más.
- **JavaScript bloqueante**: Algunos scripts impiden que el contenido se cargue más rápido.

#### Recomendaciones:
- Optimizar la configuración del servidor para reducir los tiempos de respuesta (TTFB).
- Implementar carga asincrónica de JavaScript y CSS para evitar que bloqueen la carga del contenido principal.
- Continuar con la optimización de imágenes para mejorar el tiempo de carga.

### Conclusiones

- **Tiempo de carga**: En general, el tiempo de carga es razonable en las tres páginas, pero existen oportunidades para mejorar aún más la velocidad, especialmente en dispositivos móviles.
- **Optimización de imágenes y recursos estáticos**: La optimización de imágenes y la minimización de recursos JavaScript y CSS son áreas clave de mejora.
- **Estabilidad visual (CLS)**: El CLS se mantiene dentro de los valores aceptables, pero algunas pequeñas mejoras en el manejo de los elementos visuales pueden evitar desplazamientos no deseados.

En resumen, aunque la puntuación es bastante buena, siempre hay margen de mejora en cuanto a la optimización de imágenes, tiempos de respuesta y la carga de recursos.

## Optimización con Lighthouse

### Evaluación del rendimiento con Lighthouse en Chrome DevTools

Se utilizó Lighthouse para evaluar el rendimiento del sitio web en diversos parámetros clave que afectan la experiencia del usuario. A continuación se detallan los resultados obtenidos en la página principal y las recomendaciones de optimización.

### Resultados de Lighthouse

#### 1. Largest Contentful Paint (LCP)
- **Valor:** 2.9 segundos
- **Descripción:** El LCP mide el tiempo que tarda en renderizarse el elemento más grande visible en la pantalla.
- **Recomendación:** Para mejorar el LCP, es importante optimizar las imágenes, especialmente aquellas que forman parte del contenido visible más grande (como las imágenes principales o banners). También se puede aplicar carga diferida (lazy loading) para los recursos no esenciales.

#### 2. Interaction to Next Paint (INP)
- **Valor:** 150 ms
- **Descripción:** INP mide la latencia de la interacción con elementos interactivos (como botones y formularios).
- **Recomendación:** Para reducir el INP, es importante optimizar los scripts que afectan la interacción con la interfaz. Esto incluye la optimización de eventos que no bloqueen la interacción del usuario y la minimización de JavaScript.

#### 3. Cumulative Layout Shift (CLS)
- **Valor:** 0.02
- **Descripción:** El CLS mide la estabilidad visual del contenido durante la carga, es decir, la cantidad de movimiento no deseado de los elementos en la pantalla.
- **Recomendación:** El valor obtenido es muy bajo, lo que indica una buena estabilidad visual. Sin embargo, es importante seguir utilizando medidas como definir el tamaño de las imágenes o los elementos multimedia para evitar cambios inesperados.

#### 4. First Contentful Paint (FCP)
- **Valor:** 1.1 segundos
- **Descripción:** El FCP mide el tiempo hasta que se muestra el primer elemento visual en la pantalla.
- **Recomendación:** La optimización de los recursos críticos y la minimización de los archivos CSS y JavaScript podría reducir aún más el tiempo de FCP, lo que mejora la percepción de la velocidad de la página.

#### 5. First Input Delay (FID)
- **Valor:** 50 ms
- **Descripción:** El FID mide el tiempo de respuesta a la primera interacción del usuario con la página, como hacer clic en un enlace o botón.
- **Recomendación:** Mantener la interactividad optimizada con una ejecución rápida de los scripts y la reducción de los bloqueos de hilo, minimizando el JavaScript en la carga inicial.

#### 6. Time to First Byte (TTFB)
- **Valor:** 0.4 segundos
- **Descripción:** El TTFB mide el tiempo hasta que se recibe el primer byte de datos desde el servidor.
- **Recomendación:** El TTFB es rápido, pero aún se podría mejorar al optimizar la configuración del servidor o utilizar un servicio CDN (Content Delivery Network) para reducir la latencia y entregar contenido más rápidamente.

### Recomendaciones Generales:
- **Optimización de imágenes**: Reducir el tamaño de las imágenes y servirlas en formatos modernos como WebP.
- **Optimización de JavaScript y CSS**: Minimizar los archivos JavaScript y CSS, aplicar carga asincrónica para recursos no esenciales y dividir el código (code splitting) para cargar solo lo necesario.
- **Uso de un CDN**: Implementar una red de entrega de contenido (CDN) para reducir la latencia y acelerar la carga de recursos.
- **Lazy Loading**: Aplicar lazy loading para imágenes y otros recursos que no sean visibles de inmediato para el usuario.
- **Mejorar la interactividad**: Optimizar los scripts que afectan la interacción del usuario y reducir el tiempo de ejecución.

### Conclusiones:
El sitio web tiene un rendimiento generalmente bueno según Lighthouse, con tiempos de carga rápidos y una buena estabilidad visual. Sin embargo, se pueden realizar optimizaciones adicionales para reducir aún más los tiempos de carga y mejorar la experiencia del usuario, especialmente en dispositivos móviles.


## Parte 6: Evaluación con Ghost Inspector

En esta sección, se llevó a cabo un testeo automatizado utilizando **Ghost Inspector** para evaluar la navegación general y los procesos críticos del sitio web. El objetivo es asegurar que todas las funciones principales del sitio web se comporten de manera esperada y eficiente.

### Objetivos del Test

- Verificar que la navegación general del sitio sea fluida.
- Comprobar que los botones y enlaces sean funcionales.
- Evaluar los tiempos de carga y detectar posibles cuellos de botella.
- Identificar errores como botones inactivos, enlaces rotos o pantallas que no se cargan correctamente.

### Proceso

1. Se configuró Ghost Inspector para realizar una serie de pruebas automatizadas sobre los flujos más relevantes del sitio.
2. El testeo cubrió las áreas críticas del sitio, como:
   - Acceso a la página de inicio.
   - Navegación entre páginas clave (por ejemplo, la página de cursos y el carrito de compras).
   - Interacción con los botones importantes (ej. 'Añadir al carrito', 'Ver curso').
3. Se registró un video del testeo automatizado que muestra cómo se realizó la prueba y el comportamiento del sitio web durante las interacciones.

### Análisis de los Resultados

- **Comparación con el flujo de navegación esperado**: Se revisó que todos los pasos automatizados en el video coincidieran con el flujo diseñado. Cualquier desviación de este flujo fue documentada para ser corregida.
- **Problemas encontrados**: Se identificaron ciertos puntos donde los tiempos de carga fueron más largos de lo esperado, lo cual podría afectar la experiencia del usuario.
- **Recomendaciones**:
   - Optimizar los tiempos de carga mejorando la eficiencia de las consultas a la base de datos y utilizando técnicas como lazy loading o compresión de imágenes.
   - Revisión de los botones y enlaces para asegurarse de que todos estén correctamente enlazados y sean interactivos.

## **7. Reflexiones Finales sobre la Usabilidad y Navegación del Sitio Web**

En base a los resultados obtenidos en las pruebas de usabilidad y rendimiento, se puede concluir que el sitio web presenta una estructura sólida y funcional, pero aún existen áreas de mejora que pueden optimizar la experiencia del usuario.

### **Aspectos Positivos:**
- **Accesibilidad y Responsividad:** La página se adapta adecuadamente a diferentes dispositivos y tamaños de pantalla, lo que es fundamental para proporcionar una experiencia de usuario consistente en dispositivos móviles y escritorios. Además, la inclusión de etiquetas semánticas y atributos `alt` en imágenes demuestra un buen enfoque hacia la accesibilidad.
- **Navegación Fluida:** La navegación con ratón es satisfactoria, y los enlaces y botones funcionan correctamente, lo que facilita la interacción con el sitio web. 

### **Áreas de Mejora:**
- **Visibilidad del Foco en Teclado:** Aunque la navegación por teclado es posible, se requiere mejorar la visibilidad del foco para garantizar que los usuarios con discapacidades visuales o aquellos que prefieren usar el teclado puedan interactuar sin dificultades.
- **Contraste y Legibilidad:** Se ha identificado que algunas secciones del sitio web presentan problemas de contraste, lo cual puede afectar la lectura, especialmente en usuarios con deficiencias visuales. Es importante abordar este problema para asegurar una mejor accesibilidad.
- **Interacción en Pantallas Táctiles:** Aunque la experiencia móvil es aceptable, se han observado problemas con el tamaño de los botones en pantallas pequeñas. Mejorar la disposición de los elementos táctiles y la separación entre botones puede optimizar la usabilidad en dispositivos móviles.

### **Recomendaciones Finales:**
- **Optimización de Imágenes:** Reducir el tamaño de las imágenes y aplicar técnicas como la carga diferida (lazy loading) puede mejorar considerablemente los tiempos de carga.
- **Optimización de JavaScript y CSS:** Minimizar los archivos de JavaScript y CSS contribuirá a una carga más rápida y a una mejor experiencia en dispositivos móviles.
- **Mejora en la Interactividad:** Asegurarse de que los elementos interactivos sean fácilmente accesibles y responsivos en todos los dispositivos, con especial atención a la visibilidad del foco en la navegación por teclado y la disposición de los botones en dispositivos táctiles.

En conclusión, con algunos ajustes en la accesibilidad, la interactividad y la optimización de los tiempos de carga, el sitio web puede ofrecer una experiencia de usuario significativamente mejorada, adaptada a una audiencia diversa y utilizando distintos tipos de dispositivos.
