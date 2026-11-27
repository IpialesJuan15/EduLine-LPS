# EduLine: Línea de Productos Software para Plataformas Educativas

Trabajo integrador de Ingeniería de Línea de Productos Software (LPS)
Universidad Técnica del Norte, Facultad de Ingeniería en Ciencias Aplicadas (FICA), Carrera de Software, Ibarra, Ecuador

**Autores**

- Espinoza Basantes Giuliana Alejandra (gaespinozab@utn.edu.ec)
- Huera Navarro Jhordan Marcelo (jmhueran@utn.edu.ec)
- Ipiales Ipiales Juan David (jdipialesi@utn.edu.ec)

## Descripción

EduLine es una línea de productos software para plataformas de gestión del aprendizaje (LMS). A partir de un núcleo común de activos reutilizables, permite derivar productos adaptados a escuelas, academias, universidades y empresas de capacitación. El trabajo cubre la ingeniería de dominio completa: análisis de comunalidad y variabilidad, modelo de características, arquitectura de referencia, derivación de productos y análisis económico.

## Resumen del diseño

| Elemento | Detalle |
|---|---|
| Dominio | Plataformas educativas (LMS multi-institución) |
| Portafolio | EduSchool, EduAcademy, EduCampus y EduCorp |
| Análisis C/V | 10 características comunes y 11 puntos de variación |
| Modelo FODA | 43 características, 4 grupos OR, 2 grupos XOR y 6 restricciones cross-tree |
| Herramienta | FeatureIDE |
| Arquitectura | Modelo C4, nivel 2 (contenedores), monolito modular con mecanismos de variación por punto (Strategy, Template Method, Observer, Adapter, plugins, build flavors) |
| Productos derivados | EduSchool (colegios), EduCampus (universidades) y EduCorp (capacitación corporativa) |
| Análisis económico | Modelo de Clements y Northrop: punto de equilibrio con el tercer producto y ROI de 46,8 % con cuatro productos |

## Estructura del repositorio

```
EduLine-LPS/
├── feature-model/    Modelo de características (model.xml, FeatureIDE)
├── architecture/     Arquitectura de referencia C4 (PNG y código PlantUML)
├── configs/          Configuraciones de los tres productos (.config)
└── docs/             Informe en formato IEEE, figuras y evidencias de FeatureIDE
```

## Productos derivados

| Producto | Mercado objetivo | Características | Decisiones principales |
|---|---|---|---|
| EduSchool | Colegios y escuelas pequeñas | 23 | SaaS compartido, autenticación local, foro e insignias |
| EduCampus | Universidades e institutos superiores | 32 | Instancia dedicada, SSO, LTI, calificación automática, proctoring y analítica |
| EduCorp | Capacitación corporativa | 36 | SaaS, SSO, integración con ERP, SCORM, certificación y pagos |

## Artefactos

- Modelo de características: `feature-model/model.xml`
- Arquitectura de referencia: `architecture/c4-contenedores.png`
- Configuraciones: `configs/EduSchool.config`, `configs/EduCampus.config`, `configs/EduCorp.config`
- Informe: `docs/Informe_LPS_EduLine.pdf`
