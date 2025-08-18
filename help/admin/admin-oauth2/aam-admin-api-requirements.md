---
description: Cosas que debe animar a sus clientes a tener en cuenta cuando trabajan con las API de Audience Manager.
seo-description: Things you should encourage your clients to be aware of when they're working with the Audience Manager APIs.
seo-title: API Requirements and Recommendations
title: Requisitos y recomendaciones de API
uuid: eba9cf92-f0c8-4394-8532-0de9a2e7b103
exl-id: 24f90732-31a6-436d-862b-e6871d279c7a
source-git-commit: c7c5da62b32f6a56152e1c09a965facfc601cade
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 0%

---

# Requisitos y recomendaciones de API {#api-requirements-and-recommendations}

Aspectos que debe advertir a los clientes cuando trabajan con Audience Manager [!DNL API].

## Requisitos {#requirements}

Tenga en cuenta lo siguiente al trabajar con el código [!DNL Audience Manager] [!DNL API]:

* **Parámetros de solicitud:** Todos los parámetros de solicitud son obligatorios a menos que se especifique lo contrario.
* **[!DNL JSON]tipo de contenido:** Especifique `content-type: application/json` *y* `accept: application/json` en su código.

* **Solicitudes y respuestas:** Envíe solicitudes como un objeto [!DNL JSON] correctamente formateado. [!DNL Audience Manager] responde con [!DNL JSON] datos formateados. Las respuestas del servidor pueden contener datos solicitados, un código de estado o ambos.

* **Acceso:** Su asesor de [!DNL Audience Manager] le proporcionará un identificador de cliente y una clave que le permitirán realizar [!DNL API] solicitudes.

* **Ejemplos de documentación y código:** El texto en *cursiva* representa una variable que proporciona o pasa al realizar o recibir datos de [!DNL API]. Reemplace el texto *cursiva* con su propio código, parámetros u otra información necesaria.

## Recommendations: Crear un usuario de API genérico {#recommendations}

Se recomienda crear una cuenta de usuario técnica independiente para trabajar con Audience Manager [!DNL API]. Se trata de una cuenta genérica que no está vinculada a un usuario específico de la organización del cliente ni asociada a él. Este tipo de cuenta de usuario [!DNL API] ayuda a lograr dos cosas:

* Identifique qué servicio está llamando a [!DNL API] (por ejemplo, llamadas de una aplicación cliente que usa nuestros [!DNL API]s o desde que realiza cambios masivos).
* Proporcione acceso ininterrumpido a [!DNL API]. Una cuenta vinculada a un empleado específico puede ser eliminada cuando se va de la compañía. Esto evitará que sus clientes trabajen con el código [!DNL API] disponible. Una cuenta genérica que no esté vinculada a un empleado en particular ayuda a evitar este problema.

Como ejemplo o caso de uso para este tipo de cuenta, supongamos que sus clientes desean cambiar muchos segmentos a la vez con las [herramientas de administración masiva](https://experienceleague.adobe.com/docs/audience-manager/user-guide/reference/bulk-management-tools/bulk-management-intro.html?lang=en). Para ello, necesitan acceso de [!DNL API]. En lugar de agregar permisos a un usuario específico, cree una cuenta de usuario [!DNL API] no específica que tenga las credenciales, la clave y el secreto adecuados para realizar llamadas a [!DNL API]. Esto también resulta útil si el cliente desarrolla sus propias aplicaciones que utilizan [!DNL Audience Manager] [!DNL API]s.
