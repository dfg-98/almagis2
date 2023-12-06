
# Capítulo 1: Introducción

Un Sistema de Información Geográfica (GIS, por sus siglas en inglés) es un conjunto integrado de software y hardware que permite la captura, almacenamiento, procesamiento, análisis y visualización de datos geográficamente referenciados[^1].[1] La capacidad de GIS para vincular datos geoespaciales con información descriptiva abre nuevas dimensiones en el análisis y la interpretación de datos en numerosas disciplinas. Como se ha definido, un GIS no es solo un mapa digital; es una herramienta compleja y poderosa para manejar y analizar datos georreferenciados.

## Historia y Evolución del GIS

El concepto de GIS se materializó por primera vez con el desarrollo del Canadian Geographical Information System (CGIS) en 1962, liderado por Roger Tomlinson[^2]. Este sistema fue una innovación significativa en el manejo de datos geográficos para el Inventario de Tierras de Canadá (Canada Land Inventory, CLI). A lo largo de las décadas, el GIS ha evolucionado desde sistemas basados en mainframes a sistemas más sofisticados y accesibles en computadoras personales.[2]

Con la proliferación de Internet[^3] en 1983[3] y la posterior emergencia de la World Wide Web[^4] en 1990[4], la distribución y el acceso a la información geográfica experimentaron una transformación radical. Esta transición digital facilitó el nacimiento de los Web GIS, que democratizan el acceso a herramientas GIS a través de la web, permitiendo su uso desde cualquier dispositivo con conexión a Internet y un navegador web.

## Objeto de Estudio: Web GIS

Esri[^5] define el Web GIS como un sistema de información distribuida que consta de al menos un servidor GIS y un cliente, siendo este último un navegador web, una aplicación de escritorio o una aplicación móvil. Esta tecnología emergió en Silicon Valley, California, cuando Xerox desarrolló un simple visor de mapas web en 1993. Desde entonces, los Web GIS han evolucionado hasta convertirse en plataformas sofisticadas que ofrecen una amplia gama de funcionalidades.[6]

El enfoque de este estudio es examinar los Web GIS en profundidad. Se explorará cómo estos sistemas, accesibles a través de diversas plataformas y dispositivos, representan una evolución significativa respecto a los GIS tradicionales, especialmente en términos de accesibilidad, usabilidad y alcance.

## Motivación y Justificación

El proyecto Cadic-UH en la Casa del Software, perteneciente a la facultad de Matemática y Computación de la Universidad de la Habana, ha orientado el desarrollo de AlmaGIS 2. Este Web GIS, diseñado como una aplicación web adaptable para la gestión de información geográfica junto al deseo personal por profundizar en el conocimiento de los sistemas de información geográfica y el análisis espacial constituyen la motivación principal de este trabajo.

## Requerimientos Funcionales y de Entorno

El desarrollo de AlmaGIS 2 se basará en una serie de requerimientos funcionales y de entorno específicos, detallados a continuación, para garantizar su eficacia y adaptabilidad:

1. **Visor Cartográfico Generalizado y Adaptable**: Implementación de un visor para cartografías que sea capaz de adaptarse a distintos dominios y contextos de uso.

2. **Funcionalidades Interactivas Estándar**: Inclusión de funcionalidades de interacción comunes como zoom, navegación panorámica (pan), y gestión de capas (activar/desactivar).

3. **Búsqueda y Selección de Elementos del Dominio**: Herramientas avanzadas para la búsqueda de elementos específicos dentro del dominio cartográfico. Esta función permitirá seleccionar y destacar elementos individuales dentro de un conjunto de resultados.

4. **Áreas de Interés y Consultas Asociadas**: Capacidad para seleccionar áreas de interés específicas y realizar consultas de datos relacionadas con estas áreas.

5. **Consulta de Datos Alfanuméricos**: Función para visualizar datos alfanuméricos asociados a elementos seleccionados en la cartografía, basados en el área de interés definida.

6. **Análisis Estadístico de Grupos y Variables Nominales**: Herramientas para realizar análisis estadísticos agrupados y por variables nominales, permitiendo una comprensión más profunda de los conjuntos de datos.

7. **Sistema de Autenticación y Gestión de Usuarios**: Implementación de un sistema robusto de autenticación de usuarios con capacidades administrativas para gestionar permisos y restricciones de acceso.

8. **Administración Avanzada de Datos**: Herramientas para una gestión eficiente de los datos almacenados, incluyendo la visibilidad y opacidad de las capas, así como la administración de usuarios y sus restricciones.

9. **Herramientas de Medición y Edición Cartográfica**: Inclusión de herramientas para medir distancias y áreas, así como para la edición de mapas que permitan resaltar zonas o elementos específicos.

10. **Funcionalidades de Búsqueda Diversificadas**: Capacidades de búsqueda avanzadas en el mapa para facilitar la localización y análisis de datos específicos.

11. **Generación y Extensibilidad de Reportes**: Creación de reportes de forma extensible, permitiendo la adaptación a diferentes necesidades de información.

12. **Exportación de Datos en Formatos Vectoriales**: Posibilidad de descargar geometrías resultantes de las búsquedas en formatos vectoriales como WKT y GeoJSON.

13. **Uso de Tecnologías de Código Abierto Actuales**: Aplicación de tecnologías de código abierto modernas y ampliamente utilizadas para asegurar la accesibilidad y la actualización continua del sistema.

14. **Compatibilidad Multiplataforma**: El software debe ser funcional y eficiente tanto en sistemas operativos Windows como Linux, garantizando así una amplia accesibilidad.

Estos requerimientos son fundamentales para el desarrollo de un sistema Web GIS que sea a la vez poderoso, flexible y accesible para una amplia gama de usuarios y aplicaciones. La implementación exitosa de estas características permitirá que AlmaGIS 2 se destaque como una herramienta innovadora en el campo de los sistemas de información geográfica.

Dos componentes fundamentales en un Web GIS son:

1. Visor de mapas: Aplicación web pensada para la visualización y la consulta de información geográfica  haciendo uso de los estándares de la OGC [^7]. [6]
2. Servidor de mapas (en inglés IMS: Internet Map Server): Provee cartografía a través de la red tanto en modo vectorial como con imágenes. La especificación estándar para estos servidores es la OGC WMS (Open Geospatial Consortium Web Map Service). [7]

Es posible la realización del proyecto gracias a la gran experiencia que posee La
Casa del Software en la realización de GIS y aplicaciones Web GIS. Se utilizarán
herramientas de código abierto[^8] como GeoServer, Net Core y Angular en sus versiones más recientes.

## Problema

El problema central que aborda esta investigación se articula en torno a una interrogante fundamental: ¿Cómo diseñar e implementar, utilizando buenas prácticas de programación, un sistema Web GIS que satisfaga integralmente todos los requerimientos funcionales y de entorno detallados previamente? Este desafío implica no solo la creación técnica de un sistema de información geográfica accesible a través de la web, sino también la garantía de que dicho sistema sea robusto, eficiente, y fácilmente adaptable a diversos contextos y necesidades de los usuarios.

Este desafío se desglosa en varios aspectos clave:

1. **Integración de Funcionalidades Avanzadas y Diversificadas**: Desarrollar un sistema que no solo ofrezca las funcionalidades estándar de un GIS, sino que también incorpore herramientas avanzadas de análisis y visualización de datos, adaptabilidad a distintos dominios y capacidades de interacción intuitiva para el usuario.

2. **Arquitectura Sostenible y Escalable**: Establecer una arquitectura de software que no solo atienda las necesidades actuales, sino que también sea capaz de adaptarse y escalar para futuras expansiones y mejoras, manteniendo la estabilidad y eficiencia del sistema.

3. **Interfaz de Usuario Intuitiva y Accesible**: Diseñar una interfaz que sea al mismo tiempo poderosa en capacidades técnicas y accesible para usuarios con variados niveles de experiencia en GIS, desde especialistas hasta usuarios ocasionales.

4. **Cumplimiento de Estándares de Desarrollo de Software**: Asegurar que todo el proceso de desarrollo se adhiera a las mejores prácticas y estándares de la industria del software, incluyendo la codificación, el testing, y la documentación, para garantizar un producto final de alta calidad.

5. **Integración de Tecnologías de Código Abierto**: Elegir y utilizar eficazmente tecnologías de código abierto, las cuales deben ser actuales, robustas y ampliamente soportadas, para asegurar la sostenibilidad y la interoperabilidad del sistema.

6. **Compatibilidad y Funcionamiento Multiplataforma**: Garantizar que el sistema sea completamente funcional y consistente en distintos sistemas operativos y dispositivos, lo que implica un enfoque meticuloso en el diseño de software multiplataforma.

7. **Gestión de Datos y Seguridad**: Implementar un sistema efectivo para la gestión de datos, que incluya no solo la manipulación eficiente de grandes volúmenes de datos geoespaciales sino también la seguridad y privacidad de dichos datos.

En resumen, el problema planteado no se limita a la mera implementación técnica de un Web GIS, sino que abarca la creación de un sistema integral, que sea tanto innovador en sus capacidades técnicas como accesible y útil para una amplia gama de usuarios. El objetivo es superar los retos actuales en el campo de los sistemas de información geográfica web y establecer un nuevo estándar en la funcionalidad, usabilidad y adaptabilidad de estos sistemas.

## Objetivos

### Objetivos Generales

- Diseñar e implementar un Web GIS que satisfaga todos los requerimientos funcionales y de entorno.
- Asegurar que el Web GIS sea extensible y esté construido siguiendo las mejores prácticas de programación.
- Incorporar las tecnologías más avanzadas y relevantes en el desarrollo del Web GIS.

#### Objetivos Específicos

- Analizar el estado actual de los Web GIS con funcionalidades similares a las deseadas.
- Desarrollar AlmaGIS 2, una nueva aplicación que utilice tecnologías modernas y de código abierto.
- Diseñar e implementar una arquitectura extensible que permita una gestión eficiente de usuarios y datos.
- Implementar herramientas específicas que satisfagan los requerimientos funcionales del proyecto.

### Estructura del Trabajo

Este trabajo

 se divide en los siguientes capítulos:

- **Capítulo 1**: Introducción

- **Capítulo 2**: Estado del Arte - Análisis de los Web GIS existentes.
- **Capítulo 3**: Solución Teórico-Conceptual-Computacional - Arquitectura de software y patrones de diseño utilizados.
- **Capítulo 4**: Detalles de Implementación - Tecnologías y herramientas utilizadas.
- **Capítulo 5**: Pruebas de Funcionalidad - Demostración del funcionamiento del software.
- **Capítulo 6**: Conclusiones - Reflexiones finales y posibles direcciones futuras.

Los anexos proporcionarán vistas adicionales de la aplicación y detalles técnicos que no se incluyen en los capítulos principales.

[^1]: Georreferenciación. La georreferenciación es la técnica de posicionamiento espacial de una entidad en una localización geográfica única y bien definida en un sistema de coordenadas y datum específicos.
[^2]: Roger Tomlinson. Geógrafo inglés residente en Canadá y principal artífice de los modernos GIS computarizados. Está considerado a nivel mundial como  ̈el padre de los GIS ̈.
[^3]: Internet. Conjunto descentralizado de redes de comunicación interconectadas que utilizan la familia de protocolos TCP/IP.
[^4]: Web. La World Wide Web (WWW) o red informática mundial, es un sistema de distribución de documentos de hipertexto o hipermedia interconectados y accesibles a través de Internet. Es uno de los servicios que más éxito ha tenido en internet, hasta tal punto que es habitual la confusión entre ambos términos.
[^5]: Esri. Esri (Environmental Systems Research Institute) es una empresa que actualmente desarrolla y comercializa software para Sistemas de Información Geográfica y es una de las compañías líderes a nivel mundial.
[^7]: OGC. El Open Geospatial Consortium (OGC) fue creado en 1994. Es una organización internacional sin fines de lucro comprometida con la creación de estándares abiertos e interoperables dentro de los Sistemas de Información Geográfica y la World Wide Web.
[^8]: Código abierto. Es el software distribuido y desarrollado libremente. Cualquier persona o entidad puede
utilizarlo y modificar su código fuente.

## Bibliografía

[1]: U. W.-M. Libraries, «What is GIS? - Mapping and Geographic Information Systems
(GIS) - Research Guides at University of Wisconsin-Madison,» [En línea]. Available:
<https://researchguides.library.wisc.edu/c.php?g=178144&p=1169699>. [Último
acceso: 14 Noviembre 2023].
[2]: Grindgis, «What is GIS – Definition?,» [En línea]. Available:
<https://grindgis.com/what-is-gis/what-is-gis-definition>. [Último acceso: 17 Noviembre 2023].
[3]: E. Andrews, «Who Invented the Internet? - HISTORY,» 28 octubre 2019. [En línea].
Available: <https://www.history.com/news/who-invented-the-internet>. [Último acceso:
17 Noviembre 2020].
[4]: J. Abbate, «Internet: Su evolución y sus desafíos».
[5]: P. Fu, Getting to know Web GIS (Third Edition), Esri Press (2 de julio de 2018), 2018.
[6]: G. d'Andorra, «Visor de mapas,» [En línea]. Available:
<https://www.cartografia.ad/visor-de-mapas>. [Último acceso: 30 Noviembre 2023].
[7]: M. A. d. R. @. J. S. @. Alejandro Díaz @alediator, «Servidores & Panorama
del SIG Libre,» [En línea]. Available: <https://panorama-sig-libre.readthedocs.io/es/latest/servidores/>. [Último acceso: 30 Noviembre 2023].
