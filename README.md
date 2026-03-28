# Práctica de Control de Versiones y Arquitectura de Software
**Alumno:** Cristian Aparicio Moncada  
**Semestre:** 4to Semestre - Ingeniería de Software y Sistemas Computacionales  
**Institución:** Universidad La Salle Nezahualcóyotl - Grupo 401

## 1. Mapeo de la Estructura de Directorios (Trunk, Tags y Branches)
En esta práctica se aplicó una organización profesional utilizando la jerarquía de Git en GitHub:
* **Trunk (Rama main):** Se definió como la línea de desarrollo principal y estable para la arquitectura empresarial.
* **Branches (Ramas de características):** Se creó la rama `feature-rest` para desarrollar nuevas funcionalidades de servicios web sin afectar la estabilidad del tronco principal.
* **Tags (Releases):** Se utilizó la función de etiquetas (`git tag v1.0.0`) para marcar la versión final de la entrega, simulando un despliegue de software empresarial.

## 2. El Ciclo de Trabajo en la Práctica
Se replicó el ciclo básico de desarrollo colaborativo mediante los siguientes comandos de Git:
* **Copia de trabajo local:** Realizada mediante `git clone` del repositorio remoto.
* **Actualización y cambios:** Uso de `git pull` para sincronizar y `git add`/`git commit` para el control de versiones del código fuente.
* **Fusión y Resolución de Conflictos:** Se simuló un conflicto de código entre las ramas `main` (protocolo SOAP) y `feature-rest` (protocolo REST), resolviéndolo mediante una fusión manual para integrar una arquitectura híbrida.

## 3. Aplicación de Patrones y Servicios Web
### Documentación de la API: REST vs SOAP
Para esta arquitectura, se justifica la elección de servicios **REST** sobre SOAP debido a:
* **Interoperabilidad:** Facilidad para conectar sistemas distribuidos modernos.
* **Rendimiento:** El uso de JSON reduce la carga en el ancho de banda en comparación con el XML de SOAP.
* **Flexibilidad:** Mayor facilidad de implementación en el ciclo de vida del desarrollo actual.

## 4. Nuevas Tendencias: Integración Continua
Como parte de la investigación, se analizó el uso de **GitHub Actions** para automatizar el despliegue de servicios. Esta herramienta permite que, tras cada `merge` exitoso en el Trunk, se ejecuten procesos automáticos de validación y despliegue, optimizando la entrega de software empresarial.