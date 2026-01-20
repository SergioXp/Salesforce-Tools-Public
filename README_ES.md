# Salesforce Permissions Tools

> **Toolkit avanzado para simplificar la gestión, auditoría y sincronización de metadatos de seguridad en Salesforce.**

[![Status](https://img.shields.io/badge/Status-Active-success)]() [![Stack](https://img.shields.io/badge/Python-Streamlit-blue)]() [![English](https://img.shields.io/badge/Lang-English-blue)](README.md)

**Salesforce Permissions Tools** es una suite de utilidades diseñada para administradores y arquitectos de Salesforce que necesitan ir más allá de las limitaciones del Setup estándar. Ofrece una **Interfaz Gráfica Moderna (GUI)** para operaciones masivas que normalmente requerirían scripts complejos o edición manual de XMLs.

> ⚠️ **Nota:** Este repositorio es una **demostración pública** (Landing Page) del proyecto `Salesforce-Tools`. El código fuente y los scripts de automatización se mantienen en un repositorio privado.

---

## 🚀 Características Principales

### 1. 🖥️ Interfaz Gráfica (GUI)
Olvídate de la línea de comandos. Una interfaz web limpia (construida con Streamlit) que permite:
- Seleccionar orgs conectadas vía SFDX.
- Visualizar barras de progreso en operaciones masivas.
- Descargar reportes y backups en Markdown/JSON al instante.

### 2. 🔄 Sincronización de Permisos (`Sync View`)
Sincroniza permisos de **View All** y **Modify All** entre entornos (ej: Prod -> UAT) con precisión quirúrgica.
- **Diferencial Inteligente**: Detecta qué falta y despliega solo lo necesario.
- **Categorization**: Distingue automáticamente entre objetos Estándar, Custom y de Paquetes Gestionados.
- **Modo Dry-Run**: Simula los cambios antes de desplegar para evitar errores en producción.

### 3. 🤔 Editor Masivo (`Bulk Editor`)
- **Edición en Grid**: Modifica miles de permisos (CRUD+FLS) en una interfaz tipo Excel.
- **Filtros Avanzados**: Oculta el ruido de objetos estándar no utilizados.
- **Smart Deploy**: Generación automática de `package.xml` y despliegue destructivo/aditivo según corresponda.

### 4. 🔍 Auditoría y Seguridad
- **Comparador de Perfiles**: Visualiza diferencias de permisos lado a lado (✅ vs ❌).
- **Connected Apps Monitor**: Detecta y revoca sesiones OAuth peligrosas (ej: Workbench en Prod).
- **Named Credentials Scan**: Alerta si un Sandbox tiene credenciales apuntando a endpoints de Producción.
- **Activity Auditor**: Análisis de login history para detectar licencias sin uso.

### 5. 🚑 Apex Doctor
- **Diagnóstico AI**: Analiza logs de excepción y diagnóstica la causa raíz automáticamente.
- **Source Map**: Descarga el código relevante de la Org para mostrar el contexto del error.

---

## 🛠️ Stack Tecnológico

La herramienta está construida priorizando la portabilidad y la seguridad:

- **Core**: Python 3.9+
- **GUI**: Streamlit (Web-based local interface)
- **Integration**: Salesforce CLI (`sf`) para autenticación y despliegues.
- **Deployment**: Docker-ready para ejecución en servidores o CI/CD pipelines.

---

## 🏭 Casos de Uso

1.  **Auditoría Pre-GoLive**: Verificar que UAT y PROD tienen los mismos permisos críticos.
2.  **Limpieza Técnica**: Identificar perfiles y permission sets obsoletos o vacíos.
3.  **Seguridad**: Detectar fugas de información o configuraciones inseguras en Sandboxes.

---

## 📬 Acceso y Contacto

Este toolkit es una solución propietaria desarrollada para optimizar operaciones DevOps en Salesforce.

Si te interesa utilizar estas herramientas en tu organización o ver una demostración técnica:

- **Email**: [sergiogonzalezhidalgo@gmail.com](mailto:sergiogonzalezhidalgo@gmail.com)
- **GitHub**: [@SergioXp](https://github.com/SergioXp)

---

## 👤 Autor

**Sergio González Hidalgo**
- 📧 [sergiogonzalezhidalgo@gmail.com](mailto:sergiogonzalezhidalgo@gmail.com)
