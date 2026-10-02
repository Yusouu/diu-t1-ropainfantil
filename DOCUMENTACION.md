# Documentación de la interfaz — Pequeños Pasos

## Índice
1. Justificación del diseño
2. Investigación y análisis de usuarios
3. Diseño de la interfaz
4. Validación y pruebas
5. Entrega y documentación final
6. Referencias bibliográficas

------------------

## 1. Justificación del diseño

### 1.1 Importancia del diseño centrado en el usuario
Hacer una app de ropa para niños pequeños no es fácil porque los que compran (padres,madres o abuelos) suelen ir con prisa, agobiados o con una mano ocupada. Si la app es liosa, la cierran y se van a otra tienda. Por eso hay que centrarse en lo que realmente necesitan: que sea rápido,claro y sin tonterías.

### 1.2 Objetivos y metas del proyecto
**Comprar rápido:** Que se pueda hacer una compra en menos de 2 minutos.
**Menos dudas con las tallas:** Que la gente no se equivoque de talla y luego haya que devolver las cosas (queremos bajar de un 5% los abandonos por esto).
**Que la use cualquiera:** Que tenga una tasa de acierto del 95% probándola con gente real, incluso si no son muy mañosos con el móvil.

### 1.3 Beneficios esperados
Para el usuario significa ahorrarse dolores de cabeza y tiempo libre. Para la tienda, vender más y tener menos devoluciones tontas.

-----------------

## 2. Investigación y análisis de usuarios

### 2.1 Datos demográficos y segmentación
Gente de entre 25 y 65 años. Desde mamás jóvenes con mil cosas en la cabeza hasta abuelos que quieren hacerle un regalo a su nieto y se lían con la tecnología.

### 2.2 Necesidades y comportamientos
Buscan las cosas al grano: categorías claras por edad, un buscador que funcione a la primera y no tener que meter mil datos para pagar.

### 2.3 Personas

#### Persona 1: Lucía (34 años, madre)
**Lo que hace:** Va en el metro con el móvil en una mano y el bolso en la otra intentando comprar algo rápido.
**Problema:** Va agobiada de tiempo y le aterra coger una talla que le quede pequeña al niño a los dos días.

#### Persona 2: Manuel (62 años, abuelo)
**Lo que hace:** Quiere comprarle un conjunto a su nieta recién nacida pero se marea con las webs modernas.
**Problema:** Ve mal las letras pequeñas y no entiende de meses, centímetros ni equivalencias de ropa infantil.

### 2.4 Análisis de la competencia
**Zara Kids:** Tienen fotos muy chulas y se ve limpio, pero los filtros de tallas son un rollo y hay que hacer mucho scroll. Nos quedamos con la idea de poner chips de filtro rápidos.
**Mayoral:** Muy bien ordenado por edades, pero el proceso de pago se hace eterno. Queremos simplificar los formularios al máximo.
**PatPat:** Tienen muchas ofertas pero meten demasiada publicidad y pop-ups molestos que agobian. Nuestra app será más limpia.

### 2.5 Insights y hallazgos clave
*La gente duda mucho con las tallas.* -> **Solución:** Un botón bien visible de "Guía de tallas" que abra un desplegable directamente en la ficha del producto.
*Se usa el móvil con una sola mano.**Solución:** Meter la barra de navegación y los botones importantes abajo del todo para llegar bien con el pulgar.
*Los formularios largos aburren.**Solución:** Campos de texto ordenados de Material Design 3 con avisos claros si te equivocas en algo.
*A los abuelos les cuesta leer letra pequeña.**Solución:** Usar una tipografía legible y tamaños correctos,evitando textos en miniatura.
--------------------

## 3. Diseño de la interfaz

### 3.1 Mapa de navegación
El recorrido que hace el usuario por la app es bastante directo para que no se pierda:
Desde el inicio podemos saltar al buscador, a las novedades o entrar directamente al catálogo filtrando por edad.
Al pulsar en cualquier producto del catálogo, se abre su detalle, donde se puede ver el carrusel de fotos y consultar la guía de tallas (que se despliega abajo con un bottom sheet).
Desde ahí se añade al carrito, se pasa al checkout para rellenar los datos de pago (con sus avisos si hay algún fallo) y se llega a la pantalla de confirmación.
Además, la barra de abajo permite moverse rápido entre el Inicio, el Catálogo y la pantalla de Perfil/Favoritos en cualquier momento.

### 3.2 Wireframes
Hice los bocetos en gris en Figma con el tamaño de móvil normal (360x800) para ver dónde ponía cada cosa sin marearme con los colores.

### 3.3 Guía de estilo Material Design 3
**Colores:** Usé el plugin de Material Theme con un verde azulado (#006B5F) Comprobé que los contrastes cumplen con el mínimo para que se lea perfectamente.
**Rejilla:** 4 columnas, márgenes de 16 dp y los botones táctiles grandecitos (mínimo 48x48 px) para que no cueste pulsar en pantallas pequeñas.


### 3.4 Prototipo de alta fidelidad
Monté las pantallas en Figma con los componentes de M3 y conecté todo el flujo para que se pueda comprar de principio a fin. También metí modo oscuro en un par de pantallas y la barra de navegación inferior funcionando.

--------------

## 4. Validación y pruebas

### 4.1 Metodologías de pruebas
La metodología fue simplemente mostrarle la aplicación a dos personas que estan dentro del target y decirles que busquen las prendas que necesiten, así, veremos qué facilidad tienen para usarla.
### 4.2 Feedback y resultados
**María José (57):** Encontró el pijama rápido, tardó poco más de un minuto y no tuvo ningún problema.
**Salva (32):** Se lió un segundo buscando dónde salía el error en el formulario de pago porque el aviso estaba un poco escondido.

### 4.3 Iteraciones y mejoras
Cambié el color y el tamaño del aviso de error en el formulario de Figma para que cantara más a la vista y se viera al momento. Las fotos del antes y el después están guardadas en su carpeta de iteración.

--------------

## 5. Entrega y documentación final

### 5.1 Compilación del diseño
Se han juntado todos los wireframes, los enlaces al prototipo de Figma y los estilos visuales en orden para que se pueda ver cómo evoluciona la app desde el esquema básico hasta el diseño final.

### 5.2 Justificación del diseño propuesto
Cada cosa que se ha puesto (el menú abajo, el botón de tallas rápido, los estados de error claros) se ha hecho pensando en que la gente no tiene tiempo que perder comprando ropa para sus niños.

### 5.3 Recomendaciones y pasos a seguir
**Optimización de accesibilidad:** Revisar y pulir los contrastes de color y los tamaños mínimos de texto para asegurar una lectura perfecta en cualquier dispositivo android de gama baja o media.
**Ampliación del catálogo y filtros:** Añadir opciones de filtrado más avanzadas como por tipo de tejido o temporada basándose en las demandas detectadas en el análisis de la competencia.
**Mejora del flujo de notificaciones:** Implementar avisos push para el seguimiento de envíos y alertas de reposición de tallas agotadas.
-------------

## 6. Referencias bibliográficas
Fessenden, T. (2021). *Mobile UX: Design Principles for Touch Targets*. Nielsen Norman Group.
Google. (2024). *Material Design 3 Guidelines*. Recuperado de https://m3.material.io/
Norman, D. A. (2013). *The Design of Everyday Things*. Basic Books.
Whitenton, K. (2022). *E-Commerce Product Pages for Mobile Users*. Nielsen Norman Group.
----------
**Palabra del día:** Reloj.