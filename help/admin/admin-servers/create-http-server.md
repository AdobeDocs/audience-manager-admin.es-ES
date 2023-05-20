---
description: Utilice la página Servidores de la herramienta de administración de Audience Manager para crear un nuevo servidor HTTP o para editar uno existente.
seo-description: Use the Servers page in the Audience Manager Admin tool to create a new HTTP server or to edit an existing server.
seo-title: Create or Edit an HTTP Server
title: Crear o editar un servidor HTTP
uuid: 1ef0e751-e239-4dc6-a4f6-73cc05686807
exl-id: 8b3dfb1e-2dee-4a05-835e-3c32643336bc
source-git-commit: c7c5da62b32f6a56152e1c09a965facfc601cade
workflow-type: tm+mt
source-wordcount: '302'
ht-degree: 6%

---

# Crear o editar un servidor HTTP {#create-or-edit-an-http-server}

Utilice el [!UICONTROL Servers] en la herramienta de administración de Audience Manager para crear un nuevo servidor HTTP o para editar un servidor existente.

>[!NOTE]
>
>Debe tener el [!UICONTROL DEXADMIN] para crear servidores nuevos o editar los existentes.

1. Para crear un nuevo servidor, vaya a **[!UICONTROL Servers]** > **[!UICONTROL Create Server]**. Para editar un servidor existente, haga clic en el servidor deseado en la **[!UICONTROL Label]** columna.
1. Especifique la etiqueta que desee para este servidor.
1. Desde el **[!UICONTROL Protocol]** , seleccione el protocolo que desee: [!DNL HTTP].
1. Rellene los campos:

   * **[!UICONTROL Domain]:** Especifique el dominio (host) deseado para este servidor.
   * **[!UICONTROL Port]:** Especifique el puerto deseado para este servidor. El puerto predeterminado se muestra para cada tipo de cifrado. Si es necesario, puede cambiar el puerto predeterminado
   * **[!UICONTROL Maximum Users Per Request]:** Especifique el número máximo de usuarios por solicitud permitido para este servidor.
   * **[!UICONTROL URL Prefix]:** Especifique el [!DNL URL] prefijo que se utilizará para este servidor.
   * **[!UICONTROL Authentication URL]:** Especifique el [!UICONTROL Authentication URL] para esto `HTTP` servidor.
   * **[!UICONTROL Authentication]:** Especifique el método de autenticación deseado: **[!UICONTROL None]**, **[!UICONTROL Username/Password]**, o **[!UICONTROL SSH Key]**.
   * **[!UICONTROL HTTP Signature Header]:** El nombre del [!DNL HTTP] encabezado, proporcionado por el cliente, que contiene la variable [!DNL HTTP] clave de firma. El valor predeterminado es [!UICONTROL X-Signature], como se muestra en el ejemplo siguiente:

      ```
      * Connected to partner.website.com (127.0.0.1) port 80 (#0)
      > POST /webpage HTTP/1.1
      > Host: partner.host.com
      > Accept: */*
      > Content-Type: application/json
      > Content-Length: 20
      > X-Signature: wxa2ByMWhhP328EvHQsVlOD5jTc=
      POST message content
      ```

   * **[!UICONTROL HTTP Signature Key]:** La clave utilizada para firmar el [!DNL HTTP] solicitud, proporcionada por el cliente.
   * **[!UICONTROL Show Signature Key]:** Cambie si desea mostrar o no la firma en el explorador.
   * **[!UICONTROL HTTP Signature Encryption Method]:** Especifique el método que utilizamos para cifrar la firma. Uso [!UICONTROL SHA1] a menos que el cliente prefiera lo contrario.

   >[!NOTE]
   >
   >Si desea activar [Autenticación OAuth 2.0 para transferencias de datos en tiempo real](https://experienceleague.adobe.com/docs/audience-manager/user-guide/implementation-integration-guides/receiving-audience-data/real-time-outbound-transfers/oauth-in-outbound-transfers.html?lang=en) para un socio, rellene los campos como se muestra en la tabla siguiente. Los campos de *cursiva* debe rellenarse exactamente como en la tabla.

   | Nombre  | Valor |
   |---|---|
   | [!UICONTROL Label] | [!UICONTROL Server with OAuth 2.0 enabled] |
   | [!UICONTROL Protocol] | [!UICONTROL HTTP] |
   | [!UICONTROL Domain] | [!UICONTROL api.partner.com] |
   | [!UICONTROL Port] | [!UICONTROL 443] |
   | [!UICONTROL Maximum Users per Request] | [!UICONTROL 10] |
   | [!UICONTROL URL Prefix] | [!UICONTROL /segments/aam] |
   | [!UICONTROL Authentication URL] | [!UICONTROL api.partner.com/oauth2/token] |
   | [!UICONTROL Authentication] | [!UICONTROL Username/Password] |
   | [!UICONTROL Username] | [!UICONTROL *Autorización*] |
   | [!UICONTROL Password] | your_password_here |
   | [!UICONTROL HTTP Signature Header] | [!UICONTROL Leave this field blank] |
   | [!UICONTROL HTTP Signature Key] | [!UICONTROL Leave this field blank] |
   | [!UICONTROL HTTP Signature Encryption Method] | [!UICONTROL None] |

1. Clic **[!UICONTROL Create]** si está creando un nuevo servidor, o haga clic en **[!UICONTROL Update]** si está editando un servidor existente.
