# # Tarea (a+b) · Cloud: niveles y funciones (DAW 1º)

## 🅰️ Tarea A — Niveles de cloud (IaaS/PaaS/SaaS)
Crea una tabla con 10 servicios reales. Incluye enlace oficial y justifica responsabilidades.

| Servicio | Proveedor | Nivel (IaaS/PaaS/SaaS) | Enlace oficial | ¿Qué gestiona el proveedor? | ¿Qué gestiona el equipo/usuario? |
|---------|----------|-------------------------|----------------|-----------------------------|----------------------------------|
| Amazon EC2 | AWS | IaaS | https://aws.amazon.com/ec2/ | Hardware, centros de datos, red, virtualización | Sistema operativo, apps, seguridad del SO, datos |
| Google Compute Engine | Google Cloud | IaaS | https://cloud.google.com/compute | Infraestructura física, red, hipervisor | SO, configuraciones, aplicaciones, datos |
| Azure Virtual Machines | Microsoft Azure | IaaS | https://azure.microsoft.com/services/virtual-machines/ | Infraestructura y virtualización | SO, software, seguridad, datos |
| AWS Elastic Beanstalk | AWS | PaaS | https://aws.amazon.com/elasticbeanstalk/ | Infraestructura, runtime, escalado | Código de la aplicación, configuración |
| Google App Engine | Google Cloud | PaaS | https://cloud.google.com/appengine | Plataforma, runtime, balanceo, escalado | Lógica de negocio, datos |
| Azure App Service | Microsoft Azure | PaaS | https://azure.microsoft.com/services/app-service/ | Plataforma, runtime, mantenimiento | Código, configuración, datos |
| Salesforce Sales Cloud | Salesforce | SaaS | https://www.salesforce.com/ | Aplicación completa, infraestructura, mantenimiento | Usuarios, configuración, datos |
| Google Workspace | Google | SaaS | https://workspace.google.com/ | Aplicaciones, servidores, mantenimiento | Gestión de cuentas, datos |
| Microsoft 365 | Microsoft | SaaS | https://www.microsoft.com/microsoft-365 | Software, infraestructura, actualizaciones | Usuarios, datos, permisos |
| Dropbox Business | Dropbox | SaaS | https://www.dropbox.com/business | Plataforma, almacenamiento, sincronización | Archivos, usuarios, permisos |


## 🅱️ Tarea B — Funciones principales de cloud (arquitectura)
Incluye un diagrama (ASCII/Mermaid/imagen) y una explicación breve.

### Diagrama
(Pega aquí el diagrama)
                +---------------------+
                |    Interfaz de      |
                |   Usuario / Cliente |
                |  (Web, App, API)   |
                +---------------------+
                          │
                          ▼
                +---------------------+
                |  Plataforma Cloud   |
                |  Gestión de apps,   |
                |  middleware, PaaS   |
                +---------------------+
                          │
           ┌──────────────┼───────────────┐
           ▼              ▼               ▼
   +--------------+  +-------------+ +--------------+
   | IaaS            | | PaaS      | | SaaS         |
   | Infraestructura | Plataforma  | Aplicaciones  |
   | Servidores,     | Runtime, DB | Software       |
   | almacenamiento  | Escalado    | Mantenimiento|
   +--------------+  +-------------+ +--------------+
           │              │               │
           ▼              ▼               ▼
   +-----------------------------------------------+
   |             Recursos y Datos                  |
   |  Almacenamiento, Backups, Seguridad, DB      |
   +-----------------------------------------------+


### Explicación (8–12 líneas)
(Describe el flujo front → API → BBDD/storage y dónde entra la cloud)

### Mapeo de funciones cloud a componentes (mínimo 3)
- Procesamiento → …
- Ejecución → …
- Almacenamiento → …
- Intercambio → … (opcional si ya tienes 3)

## 📚 Fuentes (enlaces oficiales)
(Enlaces oficiales usados en la tabla A y en la B)
