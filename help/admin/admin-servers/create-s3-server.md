---
description: Utilice la página Servidores de la herramienta de administración de Audience Manager para crear un nuevo servidor S3 o para editar uno existente.
seo-description: Use the Servers page in the Audience Manager Admin tool to create a new S3 server or to edit an existing server.
seo-title: Create or Edit an S3 Server
title: Creación o edición de un servidor S3
uuid: 94fee787-eb26-45aa-b602-d61ab12969ea
exl-id: 89310de0-e24e-4d4b-8171-56faf0b441f6
TQID: https://experienceleague.adobe.com/rtXpkVovwbjCwLk3caZ7Ii-LLcr2n3eL73OADaLoul0
product_v2:
  - id: df80eeb1-8d72-467e-b0df-9d51c7d3a0a1
source-git-commit: d2bed13a6ac7d38ae79b65d492b6de0ca6b6d488
workflow-type: tm+mt
source-wordcount: 211
ht-degree: 1%

---

# Creación o edición de un servidor S3 {#create-or-edit-an-s-server}

Use la página [!UICONTROL Servers] en la herramienta de administración de Audience Manager para crear un nuevo servidor [!DNL S3] o para editar uno existente.

>[!NOTE]
>
>Debe tener el rol [!UICONTROL DEXADMIN] para poder crear servidores nuevos o editar los existentes.

1. Para crear un nuevo servidor, haga clic en **[!UICONTROL Servers]** > **[!UICONTROL Create Server]**. Para editar un servidor existente, haga clic en el servidor deseado en la columna **[!UICONTROL Label]**.
1. Especifique la etiqueta que desee para este servidor.
1. En la lista desplegable **[!UICONTROL Protocol]**, seleccione el protocolo deseado: **[!UICONTROL S3]**.

   >[!NOTE]
   >
   >Se recomienda usar [!DNL Amazon S3] como método para obtener archivos de los socios y enviarlos. [!DNL Amazon S3] proporciona una interfaz de servicios web sencilla que se puede utilizar para almacenar y recuperar cualquier cantidad de datos, en cualquier momento y desde cualquier lugar de la web. Para obtener más información, consulte [Acerca de Amazon S3](https://experienceleague.adobe.com/docs/audience-manager/user-guide/reference/amazon-s3.html?lang=es) en la *Guía del usuario de Audience Manager*.

1. Rellene los campos:

   * **[!UICONTROL Account]:** Especifique la cuenta [!DNL S3] que desee.
   * **[!UICONTROL Bucket]:** Especifique el bloque [!DNL S3] deseado.
   * **[!UICONTROL Directory]:** Especifique el directorio [!DNL S3] deseado.
   * **[!UICONTROL Access Key]:** Especifique la clave de acceso [!DNL S3] que desee.
   * **[!UICONTROL Secret Key]:** Especifique la clave secreta [!DNL S3] que desee.

1. Haga clic en **[!UICONTROL Create]** si está creando un servidor nuevo, o haga clic en **[!UICONTROL Update]** si está editando un servidor existente.
