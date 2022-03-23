---
description: Para evitar la incorporación accidental de archivos y datos en fuentes de datos de destino propiedad de otros socios o clientes, el Audience Manager ha añadido un requisito de asignación entre el ID de socio (PID) y las fuentes de datos propiedad de otros socios.
title: Administrar acceso de incorporación para datos de segundo nivel
exl-id: 03bec978-dd31-41cc-a3aa-d67fbb98963c
source-git-commit: cc04863272005964cfbf1bb2319cc0dd86863680
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 0%

---

# Administrar el acceso de incorporación para datos de segundo nivel {#manage-onboarding-access-for-second-party-data}

>[!IMPORTANT]
>
> La audiencia de esta página son empleados internos del Adobe. Si es un cliente Audience Manager que solicita una asignación de fuente de datos de segundo nivel como se describe en esta página, póngase en contacto con el Servicio de atención al cliente o con el Administrador de cuentas técnico.
> Tenga en cuenta que no es necesario solicitar una asignación para las relaciones de uso compartido de datos existentes. La asignación tampoco es necesaria al incorporar datos a fuentes de datos de destino que pertenecen a su PID.

Para evitar la incorporación accidental de archivos y datos en fuentes de datos de destino propiedad de otros socios, el Audience Manager ha añadido un requisito de asignación entre el ID de socio (PID) y las fuentes de datos (DPID) propiedad de otros socios. Obtenga más información sobre PID y DPID en la [índice de ID de Audience Manager](https://experienceleague.adobe.com/docs/audience-manager/user-guide/reference/ids-in-aam.html).

Por motivos de uso compartido de datos de segundo nivel, si un socio de Audience Manager o cliente desea introducir archivos en una fuente de datos de destino que no es de su propiedad, debe solicitar una asignación entre su ID de socio (PID) y esa fuente de datos específica (DPID). Si falta la asignación, el trabajo de datos de entrada no procesa los archivos y los datos no se incorporan al Audience Manager.

Para crear esa asignación, envíe un ticket de Jira al equipo de ingeniería del Audience Manager. Ver un ticket de Jira de muestra [here](https://jira.corp.adobe.com/browse/AAM-60353). No es necesario solicitar que se creen asignaciones para ninguna relación de uso compartido de datos existente.
