---
description: Utilice la página Formatos de la herramienta de administración de Audience Manager para crear un nuevo formato o editar uno existente.
seo-description: Use the Formats page in the Audience Manager Admin tool to create a new format or to edit an existing format.
seo-title: Create or Edit a Format
title: Crear o editar un formato
uuid: ca1b1feb-bcd3-4a41-b1e8-80565f6c23ae
exl-id: 3c97d1e9-8093-4181-a1fd-fb1816cdaa3d
source-git-commit: 1f4dbf8f7b36e64c3015b98ef90b6726d0e7495a
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 1%

---

# Crear o editar un formato {#create-or-edit-a-format}

Utilice la página [!UICONTROL Formats] en la herramienta de administración de Audience Manager para crear un nuevo formato o para editar uno existente.

<!-- t_create_format.xml -->

>[!TIP]
>
>Al seleccionar un formato para los datos salientes, es mejor, si es posible, reutilizar un formato existente. El uso de un formato ya comprobado garantiza que los datos salientes se generen correctamente. Para ver exactamente el formato de un formato existente, haga clic en la opción [!UICONTROL Formats] de la barra de menús y busque el formato por nombre o por número de identificador. Los formatos o macros mal formados utilizados en formatos proporcionarán resultados con formato incorrecto o evitarán que la información se emita completamente.

1. Para crear un nuevo formato, haga clic en **[!UICONTROL Formats]** > **[!UICONTROL Add Format]**. Para editar un formato existente, haga clic en el formato deseado en la columna **[!UICONTROL Name]**.

   ![](assets/create_format.png)

1. Rellene los campos:
   * **Nombre:** (obligatorio) proporcione un nombre descriptivo para el formato.
   * **Tipo:** (obligatorio) Seleccione el formato deseado:
      * **[!UICONTROL File]**: envía datos a través de [!DNL FTP] archivos.
      * **[!UICONTROL HTTP]**: incluye datos en un contenedor de [!DNL JSON].

1. (Condicional) Si elige **[!UICONTROL File]**, rellene los campos:

   >[!NOTE]
   >
   >Para obtener una lista de las macros disponibles, consulte [Macros de formato de archivo](../formats/file-formats.md#concept_A867101505074418A58DE325949E5089) y [Macros de formato HTTP](../formats/web-formats.md#reference_C392124A5F3F42E49F8AADDBA601ADFE).

   * **[!UICONTROL File Name]:** Especifique el nombre de archivo para el archivo de transferencia de datos.
   * **Encabezado:** Especifique el texto que aparece en la primera fila del archivo de transferencia de datos.
   * **[!UICONTROL Data Row]:** Especifique el texto que aparece en cada fila saliente del archivo.
   * **[!UICONTROL Maximum File Size (In MB)]:** Especifique el tamaño máximo de archivo para los archivos de transferencia de datos. Los archivos comprimidos deben tener menos de 100 MB. No hay límite en el tamaño de archivo sin comprimir.
   * **[!UICONTROL Compression]:** Seleccione el tipo de compresión deseado: gz o zip para los archivos de datos. Para la entrega a [!UICONTROL AWS S3], debe utilizar archivos .gz o sin comprimir.
   * **[!UICONTROL .info Receipt]:** Especifica que se genera un archivo de control de transferencia ([!DNL .info]). El archivo [!DNL .info] proporciona información de metadatos acerca de las transferencias de archivos para que los socios puedan comprobar que el Audience Manager ha gestionado correctamente las transferencias de archivos. Para obtener más información, vea [Archivos de transferencia y control para transferencias de archivos de registro](https://experienceleague.adobe.com/docs/audience-manager/user-guide/implementation-integration-guides/receiving-audience-data/batch-outbound-data-transfers/transfer-control-files.html?lang=en).
   * **[!UICONTROL MD5 Checksum Receipt]:** Especifica que se genera un recibo de suma de comprobación [!DNL MD5]. El recibo de suma de comprobación [!DNL MD5] para que los socios puedan comprobar que el Audience Manager ha gestionado correctamente la transferencia completa.

1. (Condicional) Si elige **[!UICONTROL HTTP]**, rellene los campos:

   * **[!UICONTROL Method]:** Elija el método [!DNL API] que desee usar en el proceso de transferencia:
      * **[!UICONTROL POST]:** Si selecciona [!DNL POST], seleccione el tipo de contenido ([!DNL XML] o [!DNL JSON]) y después especifique el cuerpo de la solicitud.
      * **[!UICONTROL GET]:** Si selecciona [!DNL GET], especifique los parámetros de la consulta.

1. Haga clic en **[!UICONTROL Create]** si está creando un nuevo formato, o haga clic en **[!UICONTROL Save Updates]** si está editando un formato existente.

## Eliminar un formato {#delete-format}

1. Haga clic en **[!UICONTROL Formats]**.
2. Haga clic en ![](assets/icon_delete.png) en la columna **[!UICONTROL Actions]** del formato deseado.
3. Haga clic en **[!UICONTROL OK]** para confirmar la eliminación.
