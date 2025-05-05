---
description: Crear, editar y eliminar destinos de Audience Manager.
seo-description: Create, edit, and delete Audience Manager destinations.
seo-title: Manage Company Destinations
title: Administrar destinos de compañía
uuid: d9a6bfb1-7629-44e0-b7d7-ece44f65ea2b
exl-id: a2e73613-07cd-4ab8-8c6e-be451ed50bfc
source-git-commit: 79415eba732c2a6d50f04124774664f788ccc78c
workflow-type: tm+mt
source-wordcount: '1061'
ht-degree: 0%

---

# Administrar destinos de compañía {#manage-company-destinations}

Crear, editar y eliminar destinos de Audience Manager.

<!-- t_company_destinations.xml -->

Para obtener información detallada, consulte [Destinos](https://experienceleague.adobe.com/docs/audience-manager/user-guide/features/destinations/destinations.html?lang=es) en la *Guía del usuario del Audience Manager*.

## Crear o editar destinos de compañía {#create-edit-company-destinations}

Desplácese por las secciones para obtener instrucciones paso a paso sobre cómo crear nuevos destinos de [!DNL Audience Manager] o editar los existentes.

<!-- create-edit-company-destinations.xml -->

Visite la [página de integración de socios de Experience Cloud](https://wiki.corp.adobe.com/x/mPIMPw) antes de configurar destinos. La página contiene la información específica que debe rellenar para cada integración de socio [!DNL Audience Manager].

Si su cliente desea usar [!DNL Adobe Media Optimizer] como destino en [!DNL Audience Manager] , debe configurarlo en [!DNL Adobe Media Optimizer].

## Vaya a la pestaña Destinos {#navigate-destinations}

1. Haga clic en **[!UICONTROL Companies]**, luego busque y haga clic en la empresa que desee para mostrar su página [!UICONTROL Profile]. Puede usar el cuadro [!UICONTROL Search] o los controles de paginación que aparecen en la parte inferior de la lista para encontrar la compañía que desee. Puede ordenar cada columna en orden ascendente o descendente haciendo clic en el encabezado de la columna deseada.
1. Haga clic en la ficha **[!UICONTROL Destinations]**.
1. Para crear un nuevo destino, haga clic en **[!UICONTROL Add Destination]**. Para editar un destino existente, haga clic en el nombre del destino en la columna **[!UICONTROL Name]**.

## Configuración básica {#basic-settings}

Rellene los campos de la ventana **[!UICONTROL Basic Settings]**.

* **[!UICONTROL Name]:** (obligatorio) Especifique el nombre de este destino.
* **[!UICONTROL Description]:** Especifique información descriptiva sobre este destino.
* **[!UICONTROL Type]:** (obligatorio) Seleccione el tipo de destino deseado:
   * **[!UICONTROL Bulk ID]**: sincronizar ID entre distintas plataformas.
   * **[!UICONTROL Bulk Trait]**: envía información de características de forma masiva a diferentes plataformas.
   * **[!UICONTROL Bulk Segment]**: envía información de segmentos de forma masiva a diferentes plataformas.
   * **[!UICONTROL S2S]**: utilice destinos de servidor a servidor para enviar datos en tiempo real y por lotes a diferentes plataformas.
* **[!UICONTROL Auto-Fill Destination Mapping]:** ( solo [!UICONTROL S2S]) Seleccione una opción:
   * **[!UICONTROL Segment ID]:** Si selecciona esta configuración, la asignación de valor de destino se rellenará con el ID de segmento [!DNL Audience Manager].
   * **[!UICONTROL Integration Code Value]:** Si selecciona esta configuración, la asignación del valor de destino se rellenará con el código de integración de segmentos [!DNL Audience Manager].
* **[!UICONTROL User ID Key]:** (obligatorio) Seleccione la clave de ID de usuario que desee para este destino en la lista desplegable.

Este ID se utiliza como ID de la fuente de datos maestra. Esto determina los ID de usuario que deben saltar en el archivo.

>[!NOTE]
>
>Para el tipo de destino [!UICONTROL Bulk ID], no puede usar el identificador [!DNL Audience Manager] [!UICONTROL User ID] ni [!DNL Adobe Experience Cloud].

Si el identificador de origen de datos ([!UICONTROL DPID]) no se muestra en la lista desplegable, debe seleccionar la casilla de verificación **[!UICONTROL Outbound]** en el nivel de origen de datos en la [página Configuración de Data Source](https://experienceleague.adobe.com/docs/audience-manager/user-guide/features/data-sources/manage-datasources.html?lang=es).

* **[!UICONTROL Target Data Source]:** (obligatorio) Seleccione el origen de datos deseado para este destino en la lista desplegable. Esta configuración habilita el etiquetado de datos salientes, lo que permite la ingesta en sistemas independientes del lado del cliente.
* **[!UICONTROL Foreign Account ID]:** Especifique el identificador de cuenta externa para este destino. Este es el valor de identificación en el sistema del destinatario para estos datos salientes.
* **[!UICONTROL Outbound Sample Rate Denominator]:** Cuando se desconoce la cantidad total de datos devueltos, use esta configuración para devolver solamente una cantidad de datos de muestra, en lugar de la cantidad completa. Ajuste el número aquí para representar una fracción de los datos (por ejemplo, un valor de 100 devuelve 1/100 de la cantidad normal de datos, un valor de 10 devuelve 1/10 de la cantidad normal de datos). El valor predeterminado es &quot;1&quot;, que devuelve todos los datos.

## Datos en tiempo real (para destinos S2S) {#realtime-s2s}

Si está creando un destino de [!UICONTROL S2S], rellene los campos siguientes:

**[!UICONTROL Servers]**: seleccione el servidor `HTTP` deseado para este destino.
**[!UICONTROL Format]**: seleccione el formato deseado para este destino en la lista desplegable: [!UICONTROL HTTP only].

>[!NOTE]
>
>Solo para [!DNL S2S], puede habilitar o deshabilitar los destinos [!UICONTROL Realtime] o [!UICONTROL Batch] mediante los controles deslizantes de activación/desactivación en pantalla. No puede desactivar ambas opciones.

## Datos por lotes {#batch-data}

Para destinos de [!UICONTROL Bulk ID], [!UICONTROL Bulk Trait] o [!UICONTROL Bulk Segment], rellene los campos siguientes:

* **[!UICONTROL Protocol]**: (obligatorio) seleccione el protocolo deseado para este destino en la lista desplegable:
   * **[!UICONTROL FTP]**
   * **[!UICONTROL HTTP]**
   * **[!UICONTROL S3]**
* **[!UICONTROL Servers]**: (obligatorio) seleccione el servidor deseado para este destino en la lista desplegable.
* **[!UICONTROL Format]**: (Obligatorio) Seleccione el formato que desee para este destino en la lista desplegable: [!DNL HTTP] o tipo de archivo, según el protocolo que haya elegido anteriormente.
* **[!UICONTROL Sync Type]**: (obligatorio) seleccione el tipo de sincronización que desee para este destino. Esto indica el nivel de actividades de usuario que los clientes desearían incluir en los pedidos salientes. Seleccione **[!UICONTROL Customer]** si los clientes solo están interesados en analizar las clasificaciones de segmentos de sus propiedades. Seleccione **[!UICONTROL Platform]** si desea incluir clasificaciones de segmentos de actividades fuera del sitio para todos los clientes de [!DNL Audience Manager].
* **[!UICONTROL Customer]**: el archivo contiene usuarios activos que tienen al menos 1 realización de características solamente en las propiedades del cliente (asociadas con el [!UICONTROL PID] del cliente) durante el período de tiempo seleccionado. Sus clientes deben utilizar esta opción para transferir sus cualificaciones de segmento *en tiempo real* a destinos.
* **[!UICONTROL Platform]**: el archivo contiene usuarios activos que tienen al menos 1 interacción en tiempo real, ya sea sincronización de ID o realización de características, en cualquier lugar de las propiedades de todos los [!DNL Audience Manager] clientes (asociados a todos los PID de cliente) durante el período de tiempo seleccionado. Los clientes deben usar esta opción para transferir sus cualificaciones de segmento *total* a destinos.
* **[!UICONTROL Lifetime]**: el archivo contiene usuarios activos vistos en cualquier parte de las propiedades de los [!DNL Audience Manager] clientes desde la creación del destino.
* **[!UICONTROL Sync Type Lookback Period]**: si selecciona [!UICONTROL Customer] o [!UICONTROL Platform], seleccione un período de tiempo. Los archivos contienen usuarios activos para el período de tiempo seleccionado.
A continuación, seleccione el tipo de pedido. Esto indica la frecuencia y el ámbito de cada integración saliente con los socios. Seleccione entre pedidos incrementales y completos.
* **[!UICONTROL Incremental Scheduled Run]**: con cada ejecución, [!DNL Audience Manager] solo sacará de la red a los nuevos usuarios calificados desde el pedido saliente anterior. Seleccione el período de tiempo deseado en el que desea que [!DNL Audience Manager] realice procesos de sincronización incrementales. Por ejemplo, puede seleccionar cada 24 horas, cada siete días, cada 30 días o nunca.

<!--
I removed {importance="high"} from note for Exp League rendering. -Bob
-->

>[!NOTE]
>
>El primer pedido incremental es equivalente a un pedido completo porque nunca se enviaron usuarios anteriores al destino.

* **[!UICONTROL Full Sync Scheduled Run]**: con cada ejecución, [!DNL Audience Manager] saldrá de todos los usuarios activos desde que se configuró el destino por primera vez. Seleccione la programación que desee que [!DNL Audience Manager] use para realizar procesos de sincronización completos. Por ejemplo, puede seleccionar cada 24 horas, cada siete días, cada 30 días o nunca.

<!--
I removed {importance="high"} from note for Exp League rendering. -Bob
-->

>[!NOTE]
>
>Se recomienda utilizar sincronizaciones incrementales con más frecuencia que sincronizaciones completas. Las sincronizaciones incrementales solo envían archivos que contienen nuevas realizaciones de rasgos o sincronizaciones de ID. Las sincronizaciones completas envían todos los archivos, independientemente de si incluyen nuevas realizaciones o sincronizaciones de ID. Utilice únicamente la configuración [!UICONTROL Full Sync Scheduled Run] cuando los clientes necesiten una copia completa de todos sus usuarios para reducir el volumen de datos de salida.

## Configuración de fuentes de datos {#configure-data-sources}

Para destinos de [!UICONTROL Bulk ID], [!UICONTROL Bulk Trait] o [!UICONTROL Bulk Segment], rellene los campos siguientes. Esta configuración le permite enviar todos los datos (características, segmentos o ID, según el tipo seleccionado) asociados a las fuentes de datos.

* **[!UICONTROL All Unrestricted First Party Data]**: seleccione esta opción para usar todos los orígenes de datos de origen. Si selecciona esta opción, las opciones [!UICONTROL Available Data Sources] se deshabilitarán.
* **[!UICONTROL Available Data Sources]**: utilice las flechas para mover orígenes de datos entre los cuadros **[!UICONTROL Available Data Sources]** y **[!UICONTROL In File Data Sources]**.

## Guardar y finalizar {#save-and-finalize}

El botón **[!UICONTROL Save]** se activa después de rellenar todos los campos obligatorios. Haga clic en **[!UICONTROL Save]** para finalizar el proceso de creación de destino.

## Eliminar destinos de empresa {#delete-company-destinations}

<!-- delete-company-destinations.xml -->

Para eliminar un destino:

1. Haga clic en **[!UICONTROL Companies]**, busque y haga clic en la empresa que quiera y luego haga clic en la ficha **[!UICONTROL Destinations]**.
1. Haga clic en ![](assets/icon_delete.png) en la columna **[!UICONTROL Actions]** del destino deseado.
1. Haga clic en **[!UICONTROL OK]** para confirmar la eliminación.

>[!NOTE]
>
>No puede eliminar un destino si tiene segmentos asignados.
