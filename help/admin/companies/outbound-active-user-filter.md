---
description: Siga estas instrucciones para generar un archivo de sincronización completo que incluya solo usuarios activos recientemente. Es posible que desee filtrar para que los usuarios activos inserten los datos relevantes en un sistema de segmentación en el sitio o para limitar el tamaño de los archivos enviados a un DSP. No puede utilizar este filtro con sincronización incremental.
seo-description: Follow these instructions to generate a full synchronization file that includes recently active users only. You may want to filter for active users to push relevant data to an on-site targeting system or to limit the size of the files sent to a DSP. You cannot use this filter with incremental synchronization.
seo-title: Filter Outbound Data by Active Users Only
title: Filtrar datos de salida solo por usuarios activos
uuid: a2b4a385-eee3-458c-b978-09509cacb397
exl-id: d501cfd1-64dd-448e-92c5-180c0081d3e5
TQID: https://experienceleague.adobe.com/rr6ABB4pgrhkWG88VenqIcbyAaPQfbg258M6SVdE28k
product_v2:
  - id: df80eeb1-8d72-467e-b0df-9d51c7d3a0a1
feature_v2:
  - id: c814092e-2730-45e8-a12d-e084529f52cb
source-git-commit: d2bed13a6ac7d38ae79b65d492b6de0ca6b6d488
workflow-type: tm+mt
source-wordcount: 219
ht-degree: 0%

---

# Filtrar datos de salida solo por usuarios activos {#filter-outbound-data-by-active-users-only}

Siga estas instrucciones para generar un archivo de sincronización completo que incluya solo usuarios activos recientemente. Es posible que desee filtrar para que los usuarios activos inserten los datos relevantes en un sistema de segmentación en el sitio o para limitar el tamaño de los archivos enviados a un DSP. No puede utilizar este filtro con sincronización incremental.

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
