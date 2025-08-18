---
description: Utilice la página Servidores de la herramienta de administración de Audience Manager para crear un nuevo servidor FTP o para editar uno existente.
seo-description: Use the Servers page in the Audience Manager Admin tool to create a new FTP server or to edit an existing server.
seo-title: Create or Edit an FTP Server
title: Crear o editar un servidor FTP
uuid: 9273abb2-963d-4d83-bf5a-b3817f0b90e6
exl-id: 9eae4ecf-ccde-483a-ae53-1cbac033d8d6
source-git-commit: 8af040e49b881302315e0b66baa73db47c5eee28
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 1%

---

# Crear o editar un servidor FTP {#create-or-edit-an-ftp-server}

Utilice la página [!UICONTROL Servers] de la herramienta de administración de Audience Manager para crear un nuevo servidor FTP o para editar un servidor existente.

>[!NOTE]
>
>Debe tener el rol [!UICONTROL DEXADMIN] para poder crear servidores nuevos o editar los existentes.

1. Para crear un nuevo servidor, haga clic en **[!UICONTROL Servers]** > **[!UICONTROL Create Server]**. Para editar un servidor existente, haga clic en el servidor deseado en la columna **[!UICONTROL Label]**.
1. Especifique la etiqueta que desee para este servidor.
1. En la lista desplegable **[!UICONTROL Protocol]**, seleccione el protocolo deseado: **FTP**.

   >[!NOTE]
   >
   >Se recomienda usar [!DNL Amazon S3] como método para obtener archivos de los socios y enviarlos. [!DNL Amazon S3] proporciona una interfaz de servicios web sencilla que se puede utilizar para almacenar y recuperar cualquier cantidad de datos, en cualquier momento y desde cualquier lugar de la web. Para obtener más información, consulte [Acerca de Amazon S3](https://experienceleague.adobe.com/docs/audience-manager/user-guide/reference/amazon-s3.html) en la *Guía del usuario de Audience Manager*.

1. Rellene los campos:

   * **[!UICONTROL Type]:** Seleccione el tipo de cifrado deseado: **[!UICONTROL SFTP]** o **[!UICONTROL FTPs/TLS]**.
   * **[!UICONTROL Domain]:** Especifique el dominio (host) deseado para este servidor.
   * **[!UICONTROL Port]:** Especifique el puerto deseado para este servidor. El puerto predeterminado se muestra para cada tipo de cifrado. Si es necesario, puede cambiar el puerto predeterminado.
   * **[!UICONTROL Remote Path]:** Especifique la ruta de acceso remota que desee para este servidor. Si deja este campo vacío, Audience Manager coloca los archivos en el directorio predeterminado.
   * **[!UICONTROL .tmp File Rename on Completion]:** Active esta opción para cambiar el nombre del archivo `.tmp` al finalizar.
   * **[!UICONTROL Filename Suffix]:** Especifique el texto que desea anexar para transferir archivos.
   * **[!UICONTROL Moved to When Finished]:** Especifique la ruta de acceso a la ubicación a la que desea mover el archivo de transferencia al finalizar.
   * **[!UICONTROL Authentication]:** Especifique el método de autenticación de servidor deseado: **[!UICONTROL Username/Password]** o **[!UICONTROL SSH Key]**.

   >[!NOTE]
   >
   >Recuerde agregar su salida [!DNL FTP] [!DNL IP] a su lista de direcciones IP permitidas: **54.204.116.43**.

1. Para la autenticación **[!UICONTROL SSH Key]**:
   >[!NOTE]
   >
   >Al configurar la autenticación de clave SSH, asegúrese de generar siempre las claves públicas y privadas solo en formato OpenSSH.
   >1. Genere el par de claves pública y privada desde cualquier equipo [!DNL Linux] o [!DNL Mac].
   >1. Asigne la **clave pública** al cliente para que la actualice en su servidor [!DNL SFTP]. Deben incluir todo el texto de la clave pública en su servidor, incluidos `-----BEGIN RSA PRIVATE KEY-----` y `-----END RSA PRIVATE KEY-----` A cambio, deben proporcionar el nombre de usuario con el que instalan la clave.
   >1. Actualice el campo de nombre de usuario con el proporcionado por el cliente y el campo de clave con la **clave privada**.
1. Haga clic en **[!UICONTROL Create]** si está creando un servidor nuevo, o haga clic en **[!UICONTROL Update]** si está editando un servidor existente.
