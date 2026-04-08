---
description: De forma predeterminada, todas las empresas sincronizan los datos con Adobe Media Optimizer (AMO). En la IU de administración, cada contenedor de compañía tiene una fuente de datos que administra este proceso. Esta fuente de datos es Adobe AMO (ID 411). Haga clic en una fila de contenedor (en la pestaña Contenedores ) de una empresa seleccionada para deshabilitar esta sincronización predeterminada o para agregar y quitar otras fuentes de datos al proceso de sincronización de AMO.
seo-description: By default, all companies sync data with Adobe Media Optimizer (AMO). In the Admin UI, each company container has a data source that manages this process. This data source is Adobe AMO (ID 411). Click a container row (under the Containers tab) for a selected company to disable this default sync or to add and remove other data sources to the AMO sync process.
seo-title: ID Syncing with Media Optimizer
title: Sincronización de ID con Media Optimizer
uuid: b741dfa7-2947-4288-b214-79eccf18d53a
exl-id: ebd978ef-3825-4a96-94bd-5cdae269cf7c
TQID: https://experienceleague.adobe.com/R6xtPWC964J1atGK-R0g6J5AG83PYJosHNE3-5LvMVE
product_v2: id: df80eeb1-8d72-467e-b0df-9d51c7d3a0a1
source-git-commit: d2bed13a6ac7d38ae79b65d492b6de0ca6b6d488
workflow-type: tm+mt
source-wordcount: 222
ht-degree: 2%

---

# Sincronización de ID con Media Optimizer {#id-syncing-with-media-optimizer}

De manera predeterminada, todas las empresas sincronizan los datos con [!DNL Adobe Media Optimizer] ([!DNL AMO]). En [!UICONTROL Admin UI], cada contenedor de compañía tiene un origen de datos que administra este proceso. Este origen de datos es [!UICONTROL Adobe AMO] ([!UICONTROL ID] 411). Haga clic en una fila de contenedor (en la ficha [!UICONTROL Containers]) de una empresa seleccionada para deshabilitar esta sincronización predeterminada o para agregar y quitar otras fuentes de datos al proceso de sincronización de [!DNL AMO].

![](assets/id-sync.png)

## Estado de sincronización de ID {#id-sync-status}

En la tabla siguiente se describe el estado de sincronización de un origen de datos.

| Estado | Descripción |
|------ | -------- |
| Off | Quite todos los orígenes de datos de [!UICONTROL Selected Data Sources] para este contenedor con el fin de deshabilitar la sincronización de ID con [!DNL AMO] |
| Activado (independientemente de la versión del servicio de ID) | Una fuente de datos se sincroniza con [!DNL AMO] independientemente de la versión del servicio de ID cuando: <ul><li>El origen de datos aparece en la lista [!UICONTROL Selected Data Sources].</li><li>La casilla de verificación [!DNL AMO] *no está* seleccionada.</li></ul> |
| Activado (independientemente de la versión del servicio de ID) | Se sincronizará un origen de datos con [!DNL AMO] con la versión 2.0 (o posterior) del servicio de ID cuando: <ul><li>El origen de datos aparece en la lista [!UICONTROL Selected Data Sources].</li><li>La casilla de verificación [!DNL AMO] *está* seleccionada.</li></ul> |

>[!MORELIKETHIS]
>
>* [Administrar contenedores](../companies/admin-manage-containers.md#task_61DB5CEECC5049DD8D059C642AC3F967)
