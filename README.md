# Práctica de Arquitectura de Software - SROP
**Crstian Aparicio MOncada 
**Semestre:** 4to Semestre - Ingeniería de Software y Sistemas Computacionales  
**Institución:** Universidad La Salle Nezahualcóyotl

## 1. Estructura de Control de Versiones
Para este proyecto se implementó una jerarquía profesional basada en:
* **Trunk (Main):** Línea de desarrollo principal y estable de la arquitectura.
* **Branches (Feature Branches):** Uso de ramas paralelas (ej. `feature-rest`) para el desarrollo de servicios web sin afectar el tronco principal.
* **Tags (Releases):** Marcado de versiones finales (v1.0.0) para el despliegue empresarial.

## 2. Aplicación de Patrones y Servicios Web
### Justificación de Interoperabilidad: REST vs SOAP
En la arquitectura desarrollada, se ha optado por un diseño basado en **REST (Representational State Transfer)** por las siguientes razones:
* **Rendimiento:** Menor consumo de ancho de banda al utilizar JSON en lugar del XML pesado de SOAP.
* **Escalabilidad:** Ideal para servicios distribuidos y aplicaciones móviles.
* **Interoperabilidad:** Facilidad de integración con diversas plataformas modernas mediante métodos HTTP estándar.

*Nota: Durante la práctica se simuló una arquitectura híbrida resolviendo un conflicto de fusión con servicios SOAP legados.*

## 3. Integración Continua (Nuevas Tendencias)
Se investigó la implementación de **GitHub Actions** para automatizar el ciclo de vida del software. Mediante flujos de trabajo (Workflows), es posible ejecutar pruebas automáticas y despliegues en servicios como Firebase o Netlify cada vez que se realiza un `push` a la rama `main`, garantizando la estabilidad de la arquitectura empresarial.