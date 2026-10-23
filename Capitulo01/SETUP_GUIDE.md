# Setup Guide — Laboratorio MS-4019.3: agente de SharePoint

Esta guía prepara un entorno de Microsoft 365 para ejecutar la [práctica de creación y prueba del agente](README.md). El laboratorio se ejecuta en línea y utiliza siete documentos PDF de ejemplo. Esta preparación debe realizarse antes de empezar los 80 minutos de práctica.

## 1. Descripción del entorno

Se necesita un entorno organizacional de SharePoint Online moderno, con capacidad para crear agentes de SharePoint y acceder a ellos desde la aplicación Microsoft 365 Copilot. No se utilizan máquinas virtuales, servidores locales, SDK, programación, bases de datos ni servicios externos.

Los PDF pertenecen a un caso creado para el laboratorio y no contienen políticas reales de una entidad financiera. Cárgalos en una ubicación autorizada de SharePoint donde solo tengan acceso los participantes y responsables correspondientes. No incorpores direcciones internas del tenant, credenciales o datos privados en las guías o los archivos distribuidos.

## 2. Requisitos de hardware

Un equipo capaz de ejecutar un navegador moderno y una conexión estable a internet. No se requiere hardware adicional ni características especiales de CPU, RAM, almacenamiento, virtualización o periféricos.

## 3. Requisitos de software y plataforma

| Elemento | Requisito |
|---|---|
| Sistema operativo | Cualquier sistema operativo compatible con un navegador web actualizado. |
| Navegador | Microsoft Edge, Google Chrome u otro navegador actualizado y admitido por Microsoft 365. |
| SharePoint | SharePoint Online, en un sitio moderno al que el usuario pueda acceder y editar. |
| Agentes | Experiencia de creación, edición y uso de agentes de SharePoint habilitada en la organización. |
| Microsoft 365 Copilot | Acceso a la aplicación desde [m365.cloud.microsoft](https://m365.cloud.microsoft/), con la misma identidad que en SharePoint. |
| Recursos | Siete PDF del directorio `recursos/` de este paquete. |

No se requieren instalaciones de escritorio. PDF es un tipo de documento compatible como origen de agentes de SharePoint según la documentación vigente.

## 4. Cuentas, licencias, permisos y consideraciones de costos

1. Usa una cuenta de trabajo o escuela de Microsoft 365, no una cuenta personal.
2. El temario de capacitación solicita licenciamiento «M365 Copilot Premium». La denominación comercial que utiliza Microsoft es Microsoft 365 Copilot. Para reproducir el flujo completo del temario, verifica que la cuenta tenga la licencia requerida, que el plan de servicio permita Copilot en SharePoint y que la organización permita usar agentes.
3. Microsoft también documenta la alternativa de pago por uso para agentes de SharePoint, si el administrador la ha habilitado. Esta opción puede generar cargos y sus posibilidades de integración y acceso deben comprobarse para el tenant específico; no se presume que sustituye todas las experiencias del curso con licencia completa.
4. Para crear o editar agentes se necesitan permisos de edición en el sitio de SharePoint. Debes poder leer los siete documentos elegidos como conocimiento. Para cargar los recursos, necesitarás permiso de carga en la biblioteca o el apoyo de su propietario.
5. Verifica con el administrador que la creación y el uso de agentes, así como el acceso desde Microsoft 365 Copilot, no estén bloqueados por políticas del tenant.
6. No uses credenciales compartidas. No amplíes permisos ni actives facturación sin autorización.

Comprobación de licencias y permisos: entra a SharePoint con la cuenta de laboratorio, abre la biblioteca y comprueba si existe Copilot > Crear un agente o Crear un agente en el menú contextual de una selección de archivos. Si no aparece, verifica primero roles, licencia y política del servicio.

## 5. Preparar la biblioteca con los archivos del caso

### 5.1. Ubicación de trabajo

1. Accede a un sitio moderno de SharePoint autorizado para ejercicios. Un propietario con permiso suficiente puede utilizar un sitio existente o crear uno de laboratorio según la política de su organización.
2. En Documentos (o la biblioteca aprobada), crea una carpeta denominada `MS4019-Solicitudes`, si no existe una biblioteca exclusiva para este laboratorio.
3. La carpeta de trabajo debe contener solo los siete PDF indicados a continuación. Esto facilita delimitar las fuentes del agente y evita mezclar el caso con otros archivos de la organización. No pongas allí instrucciones de acceso, credenciales ni datos productivos.

### 5.2. Archivos que deben cargarse

Desde el paquete descargado, selecciona los siguientes archivos en `recursos/`, y cárgalos a la carpeta o biblioteca del laboratorio:

| Archivo | Tipo de información |
|---|---|
| `PR-SOL-01-Procedimiento-Solicitudes.pdf` | Procedimiento de atención y estados de revisión. |
| `POL-SEG-02-Politica-Servicios.pdf` | Política de acceso y autorizaciones. |
| `MR-SOL-01-Matriz-Requisitos.pdf` | Requisitos por tipo de solicitud. |
| `MR-ROL-01-Matriz-Roles.pdf` | Roles y responsabilidades. |
| `ACC-2026-104-Expediente-Acceso.pdf` | Expediente ACC con todos los soportes requeridos. |
| `HAB-2026-221-Expediente-Habilitacion.pdf` | Expediente HAB con ausencia de concepto de Seguridad TI. |
| `CAM-2026-309-Expediente-Cambio.pdf` | Expediente CAM con contradicciones entre formulario y anexos. |

4. Espera a que SharePoint confirme la carga de los siete archivos.
5. Abre cada PDF desde SharePoint, al menos una vez, y confirma que el texto y los anexos son legibles. Los documentos tienen texto seleccionable; si alguno no abre, vuelve a cargarlo.
6. Si la organización exige etiquetado, retención o controles de acceso, aplícalos de acuerdo con sus reglas. Utiliza solo permisos autorizados de lectura y edición.

### 5.3. Controlar el ámbito del agente

El agente podrá crearse después a partir de los siete PDF, de su carpeta dedicada o de una biblioteca que solo contenga el caso. En la edición del agente, comprueba que Orígenes no incluya carpetas o sitios con archivos ajenos. SharePoint respeta los permisos de cada usuario; compartir el agente no cambia esos permisos.

La documentación Microsoft indica un límite de hasta 20 elementos de origen (archivos, sitios, bibliotecas, carpetas o listas); los siete PDF de este laboratorio caben dentro del límite.

## 6. Comprobación final del alistamiento

Realiza estas pruebas funcionales sin crear informes ni registros:

1. Acceso: abre el sitio con la cuenta de laboratorio, entra a la carpeta `MS4019-Solicitudes` y abre los siete PDF.
2. Fuentes: confirma que la carpeta solo contiene estos siete archivos y que ninguno pertenece a operaciones reales.
3. Permisos de creación: confirma que el menú de SharePoint ofrece la posibilidad de Crear un agente. No crees aún el agente si deseas seguir la secuencia de la práctica.
4. Copilot: abre [Microsoft 365 Copilot](https://m365.cloud.microsoft/) con la misma cuenta y comprueba que puedes acceder a la interfaz empresarial y a la experiencia de agentes permitida.

Si se superan las comprobaciones anteriores, comienza la [práctica de 80 minutos](README.md).

## 7. Fallas frecuentes, seguridad y limpieza

- Si no aparece Crear un agente, revisa licencia, habilitación por el administrador, permisos de edición y el uso de un sitio moderno. No intentes evadir la política del tenant.
- Si los archivos no aparecen en Orígenes, comprueba los permisos y que la carga se completó. Puede existir un retraso temporal hasta que SharePoint ponga a disposición un documento recién cargado.
- Si el agente no figura en la aplicación Copilot, utiliza primero el vínculo o la conversación en SharePoint; verifica la identidad y las políticas de publicación y acceso de tu organización.
- Mantén los PDF del caso dentro del espacio autorizado. No cargues datos bancarios reales, información personal real ni credenciales.
- Al finalizar, el propietario del sitio puede eliminar los agentes o archivos del laboratorio según las políticas organizacionales, sin afectar otras bibliotecas o agentes.
- No existe necesidad de aprovisionar Azure, Copilot Studio ni máquinas virtuales para esta práctica.

## 8. Vigencia de las instrucciones y referencias oficiales

Instrucciones contrastadas con documentación de Microsoft el 23/10/2026. Microsoft anuncia una modernización de los agentes de SharePoint a partir de mediados de noviembre de 2026, con una transición desde archivos `.agent` hacia experiencias integradas con Microsoft Copilot Agent Builder. Microsoft indica que los agentes antiguos `.agent` continúan funcionando hasta finales de marzo de 2027. Por eso, antes de impartir el laboratorio en una fecha posterior, verifica que el tenant siga mostrando los controles de creación y edición descritos. No modifiques la metodología del curso sin validar el nuevo recorrido.

Referencias:

- [Crear un agente en SharePoint — Microsoft](https://support.microsoft.com/es-es/sharepoint/copilot-in-sharepoint/create-an-agent-in-sharepoint)
- [Editar un agente en SharePoint — Microsoft](https://support.microsoft.com/es-es/sharepoint/copilot-in-sharepoint/edit-an-agent-in-sharepoint)
- [Preguntas frecuentes, fuentes y formatos — Microsoft](https://support.microsoft.com/en-us/sharepoint/copilot-in-sharepoint/frequently-asked-questions-about-copilot-in-sharepoint)
- [Usar un agente de SharePoint en Copilot — Microsoft](https://support.microsoft.com/es-es/sharepoint/copilot-in-sharepoint/use-an-agent-created-in-sharepoint-in-microsoft-365-copilot-chat)
- [Actualizaciones de los agentes en SharePoint y OneDrive — Microsoft](https://learn.microsoft.com/en-us/sharepoint/upgrade-sharepoint-agents)

[Ir a la práctica](README.md)
