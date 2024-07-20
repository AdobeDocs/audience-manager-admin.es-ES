---
description: Siga estas instrucciones para generar un archivo de sincronización completo que incluya solo usuarios activos recientemente. DSP Es posible que desee filtrar para que los usuarios activos inserten los datos relevantes en un sistema de segmentación en el sitio o para limitar el tamaño de los archivos enviados a un grupo de destinatarios de un sitio de destino No puede utilizar este filtro con sincronización incremental.
seo-description: Follow these instructions to generate a full synchronization file that includes recently active users only. You may want to filter for active users to push relevant data to an on-site targeting system or to limit the size of the files sent to a DSP. You cannot use this filter with incremental synchronization.
seo-title: Filter Outbound Data by Active Users Only
title: Filtrar datos de salida solo por usuarios activos
uuid: a2b4a385-eee3-458c-b978-09509cacb397
exl-id: d501cfd1-64dd-448e-92c5-180c0081d3e5
source-git-commit: f5d74995f0664cf63e68b46f1f3c608f34df0e80
workflow-type: tm+mt
source-wordcount: '217'
ht-degree: 0%

---

# Filtrar datos de salida solo por usuarios activos {#filter-outbound-data-by-active-users-only}

Siga estas instrucciones para generar un archivo de sincronización completo que incluya solo usuarios activos recientemente. DSP Es posible que desee filtrar para que los usuarios activos inserten los datos relevantes en un sistema de segmentación en el sitio o para limitar el tamaño de los archivos enviados a un grupo de destinatarios de un sitio de destino No puede utilizar este filtro con sincronización incremental.

>[!NOTE]
>
>No es necesario ver un visitante en el sitio de un cliente seleccionado ni en el tráfico de su anuncio para que se pueda considerar &quot;activo&quot;. Cualquier cliente o socio de [!DNL Audience Manager] puede verlas para calificarlas como &quot;activas&quot;.

Para filtrar solo por usuarios activos:

1. Haga clic en **[!UICONTROL Companies]**.
1. Seleccione la empresa con la que desea trabajar y haga clic en **[!UICONTROL Destinations]**.
1. En la sección [!UICONTROL Batch Data], defina las siguientes opciones:

   * **[!UICONTROL Sync Type]**: seleccione **[!UICONTROL Customer]** o **[!UICONTROL Platform]**.
   * **[!UICONTROL Sync Type Lookback Period]**: este intervalo de tiempo define el intervalo del archivo de datos. Las opciones incluyen **[!UICONTROL 24 hours]**, **[!UICONTROL 7 days]**, **[!UICONTROL 30 days]**.
   * **[!UICONTROL Incremental Sync Scheduled Run]**: seleccione **[!UICONTROL Never]**. Recuerde, este filtro se aplica solo a archivos de sincronización completos.
   * **[!UICONTROL Full Sync Scheduled Run]**: esto determina la frecuencia con la que desea recibir este archivo. Las opciones incluyen **[!UICONTROL 24 hours]**, **[!UICONTROL 7 days]**, **[!UICONTROL 30 days]** o **[!UICONTROL Never]** (para deshabilitar).

1. Haga clic en **[!UICONTROL Save]**.
