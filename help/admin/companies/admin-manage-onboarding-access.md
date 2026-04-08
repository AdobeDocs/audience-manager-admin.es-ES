---
description: Para evitar la incorporación accidental de archivos y datos en fuentes de datos de destino propiedad de otros socios o clientes, Audience Manager ha añadido un requisito de asignación entre el ID del socio (PID) y las fuentes de datos propiedad de otros socios.
title: Administrar el acceso de incorporación para datos de segundo nivel
exl-id: 03bec978-dd31-41cc-a3aa-d67fbb98963c
TQID: https://experienceleague.adobe.com/ajdpBCvsikCo-lxT98GNrwCyc2IW-AZCg73oU18leTY
product_v2:
  - id: df80eeb1-8d72-467e-b0df-9d51c7d3a0a1
source-git-commit: d2bed13a6ac7d38ae79b65d492b6de0ca6b6d488
workflow-type: tm+mt
source-wordcount: 293
ht-degree: 0%

---

# Administrar el acceso de incorporación para datos de segundo nivel {#manage-onboarding-access-for-second-party-data}

>[!IMPORTANT]
>
> La audiencia de esta página son empleados internos de Adobe. Si es cliente de Audience Manager y solicita una asignación de fuente de datos de segundo nivel como se describe en esta página, póngase en contacto con el Servicio de atención al cliente o con el administrador de cuentas técnico.
> Tenga en cuenta que no es necesario para solicitar una asignación para las relaciones de uso compartido de datos existentes. La asignación tampoco es obligatoria al incorporar datos en fuentes de datos de destino que pertenecen a su PID.

Para evitar la incorporación accidental de archivos y datos en fuentes de datos de destino propiedad de otros socios, Audience Manager ha añadido un requisito de asignación entre el ID del socio (PID) y las fuentes de datos (DPID) propiedad de otros socios. Obtenga más información sobre PID y DPID en el [índice de Audience Manager ID](https://experienceleague.adobe.com/docs/audience-manager/user-guide/reference/ids-in-aam.html?lang=es).

Para fines de uso compartido de datos de segundo nivel, si un socio o cliente de Audience Manager desea introducir archivos en una fuente de datos de destino de la que no es propietario, debe solicitar una asignación entre su ID de socio (PID) y esa fuente de datos específica (DPID). Si falta la asignación, el trabajo de datos de entrada no procesará los archivos y los datos no se incorporarán a Audience Manager.

Para crear esa asignación, envíe un ticket Jira al equipo de ingeniería de Audience Manager. Vea un ejemplo de un ticket de Jira [aquí](https://jira.corp.adobe.com/browse/AAM-60353). No es necesario que solicite que se creen asignaciones para ninguna relación de uso compartido de datos existente.
