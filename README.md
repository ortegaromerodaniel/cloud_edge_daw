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

El flujo **front → API → BBDD/storage** sigue estos pasos: el **front-end** (UI) realiza una solicitud HTTP a la **API** cuando el usuario interactúa con la aplicación. La **API** procesa la solicitud, aplica la lógica de negocio y accede a la **base de datos** o **almacenamiento** (BBDD) para obtener o modificar datos. La **base de datos** responde con la información solicitada, y la **API** devuelve la respuesta al front-end, que la muestra al usuario.

La **cloud** entra en cada etapa: la **API** y la **base de datos** suelen estar alojadas en la nube (AWS, Google Cloud, Azure), permitiendo escalabilidad, seguridad y almacenamiento gestionado. La nube también optimiza la distribución de carga y la alta disponibilidad, asegurando que el sistema sea eficiente y resiliente ante picos de tráfico.


### Mapeo de funciones cloud a componentes (mínimo 3)
- **Procesamiento → API / Backend**
  La cloud ejecuta la lógica de negocio (validaciones, reglas, cálculos) mediante servicios como APIs, contenedores o funciones serverless.

- **Ejecución → Compute en la nube**
  El código del backend se ejecuta en recursos cloud (VMs, contenedores, Lambdas/Functions), que escalan automáticamente según la demanda.

- **Almacenamiento → BBDD / Storage cloud**
  Los datos se guardan en bases de datos gestionadas o en storage de objetos (SQL/NoSQL, blobs, buckets), garantizando persistencia y disponibilidad.

- **Intercambio → Red y servicios de comunicación**
  La cloud facilita la comunicación entre front, API y BBDD mediante redes, balanceadores y APIs expuestas de forma segura.


## 📚 Fuentes (enlaces oficiales)
(Enlaces oficiales usados en la tabla A y en la B)

Enlaces de la tabla A

* Amazon EC2 → [https://aws.amazon.com/ec2/](https://aws.amazon.com/ec2/)
* Google Compute Engine → [https://cloud.google.com/compute](https://cloud.google.com/compute)
* Azure Virtual Machines → [https://azure.microsoft.com/services/virtual-machines/](https://azure.microsoft.com/services/virtual-machines/)
* AWS Elastic Beanstalk → [https://aws.amazon.com/elasticbeanstalk/](https://aws.amazon.com/elasticbeanstalk/)
* Google App Engine → [https://cloud.google.com/appengine](https://cloud.google.com/appengine)
* Azure App Service → [https://azure.microsoft.com/services/app-service/](https://azure.microsoft.com/services/app-service/)
* Salesforce Sales Cloud → [https://www.salesforce.com/](https://www.salesforce.com/)
* Google Workspace → [https://workspace.google.com/](https://workspace.google.com/)
* Microsoft 365 → [https://www.microsoft.com/microsoft-365](https://www.microsoft.com/microsoft-365)
* Dropbox Business → [https://www.dropbox.com/business](https://www.dropbox.com/business)

Enlaces de la tabla B
* Amazon EC2: https://aws.amazon.com/ec2/
* Google Compute Engine: https://cloud.google.com/compute
* Azure Virtual Machines: https://azure.microsoft.com/services/virtual-machines/
* PaaS (Plataforma, Runtime, DB, Escalado)
* AWS Elastic Beanstalk: https://aws.amazon.com/elasticbeanstalk/
* Google App Engine: https://cloud.google.com/appengine
* Azure App Service: https://azure.microsoft.com/services/app-service/
* SaaS (Software, Aplicaciones, Mantenimiento)
* Salesforce Sales Cloud: https://www.salesforce.com/
* Google Workspace: https://workspace.google.com/
* Microsoft 365: https://www.microsoft.com/microsoft-365
* Dropbox Business: https://www.dropbox.com/business
* Recursos y Datos (Almacenamiento, Backups, Seguridad, DB)
* AWS RDS (https://aws.amazon.com/rds/)
* Google Cloud Storage (https://cloud.google.com/storage)
* Azure Blob Storage (https://azure.microsoft.com/services/storage/blobs/) gestiona recursos y datos.

