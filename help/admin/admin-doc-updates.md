---
description: Todas las actualizaciones (adiciones, eliminaciones y correcciones) realizadas por fecha en la Guía de administración de Audience Manager.
seo-description: All updates (additions, deletions, and corrections) to the Audience Manager Admin Guide, by date.
seo-title: Documentation Updates
title: Actualizaciones de documentación
uuid: 1c02dff5-8e3f-42bf-a50c-03b75e121ac7
exl-id: 8221b4df-99c2-47d3-a2ea-186a701a2b20
source-git-commit: 1f4dbf8f7b36e64c3015b98ef90b6726d0e7495a
workflow-type: tm+mt
source-wordcount: '583'
ht-degree: 94%

---

# Actualizaciones de documentación {#documentation-updates}

Todas las actualizaciones (adiciones, eliminaciones y correcciones) realizadas por fecha en la Guía de administración de Audience Manager.

Para obtener información sobre las versiones, mejoras y correcciones de errores de las funciones, consulte las [Notas de la versión de Experience Cloud](https://experienceleague.adobe.com/docs/release-notes/experience-cloud/current.html?lang=es). Para ver [!DNL Audience Manager] cambios de documentación, consulte [Actualizaciones de documentación](https://experienceleague.adobe.com/docs/audience-manager/user-guide/documentation-updates/docs-2019.html?lang=es).

## Actualizaciones de documentación de AAM 2019 {#aam-2019-docs-updates}

| Tema | Descripción |
|--- |--- |
| Macros de formato HTTP | Hemos añadido una nueva macro, `REGION_ID_LIST`, y tres campos nuevos `sda`, `sda` y `sda` a la macro `USER_LIST`. |
| Macros de formato HTTP | Hemos añadido dos nuevas macros: `ECID` y `MCID`. |

## Actualizaciones de documentación de AAM 2018 {#aam-2018-docs-updates}

<!-- c_doc_updates.xml -->

<table id="table_AECF59E131F84E7791A5A421BFB203FA"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Tema </th> 
   <th colname="col2" class="entry"> Descripción </th> 
  </tr>
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p><a href="admin-servers/create-ftp-server.md#task_BF1DD0E5ECA64AEC87EACABFCAEA2C6D"> Crear o editar un servidor FTP</a> </p> </td> 
   <td colname="col2"> <p>Hemos añadido más información sobre la autenticación de claves SSH para los servidores SFTP (paso 5). </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p><a href="admin-destination-troubleshooting.md#set-up-destinations-export"> Cómo configurar sus destinos para exportar Experience Cloud...</a> </p> </td> 
   <td colname="col2"> <p>Esta página muestra cómo configurar destinos para exportar datos con claves del tipo de ID que desee en archivos de datos de salida. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p><a href="admin-servers/admin-authorize-s3-cross-bucket.md#task_20B12994C5484A9D8CC40DF6F456CBE7"> Cómo autorizar el acceso de bloques de Amazon S3 entre cuentas para destinos por lotes</a> </p> </td> 
   <td colname="col2"> <p>Nuestros clientes pueden usar permisos de bloques entre cuentas en Amazon S3 para entregar archivos de datos de salida si no desean compartir las claves de acceso y de secreto de Amazon S3. Este documento muestra cómo configurar esta alternativa en la IU del administrador de Audience Manager. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Actualizaciones de documentación de AAM 2017 {#aam-2017-docs-updates}

<table id="table_81D2DA9293A9417085C630D00A7C96E1"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Tema </th> 
   <th colname="col2" class="entry"> Descripción </th> 
  </tr>
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"><a href="formats/web-formats.md#reference_C392124A5F3F42E49F8AADDBA601ADFE"> Macros de formato HTTP</a> </td> 
   <td colname="col2">Se ha reemplazado la macro <code>segmentId</code> por <code>legacySegmentId</code> y se ha añadido la macro <code>newSegmentId</code>. </td> 
  </tr> 
  <tr> 
   <td colname="col1"><a href="companies/admin-company-limits.md#task_3004C10CB9A9430A8D25E25BB830B5D6"> Administrar los límites de la compañía</a> </td> 
   <td colname="col2"> Se ha añadido la cantidad máxima de carpetas de características y la profundidad de la estructura de características en la documentación de límites. </td> 
  </tr> 
  <tr> 
   <td colname="col1"><a href="formats/enable-outbound-seq.md#concept_526744C9433F40BF8269E18245B2F0BD"> Habilitar las transferencias salientes de archivos de secuencias de Hadoop</a> </td> 
   <td colname="col2"> Consulte cómo puede permitir que los clientes envíen archivos SEQ de salida a su propia instancia de Hadoop. </td> 
  </tr> 
  <tr> 
   <td colname="col1"><a href="companies/admin-manage-containers.md#task_61DB5CEECC5049DD8D059C642AC3F967"> Administrar contenedores</a> </td> 
   <td colname="col2"> Se ha añadido una breve instrucción sobre cómo crear contenedores. </td> 
  </tr> 
  <tr> 
   <td colname="col1"><a href="companies/admin-manage-company-destinations.md#create-edit-company-destinations"> Crear o editar destinos de compañía</a> </td> 
   <td colname="col2"> <p> 
     <ul id="ul_527E0E75C03846B0AB39EEE544904BE2"> 
      <li id="li_FC276B34158D44E3A5450C6C8BAF3184">Se han añadido instrucciones sobre cómo equilibrar el uso de las sincronizaciones completas e incrementales. </li> 
      <li id="li_3975DA78DE9E441D8F8CB80F752DD7B7">El aprovisionamiento de <span class="keyword"> Adobe Media Optimizer</span> como destino de <span class="keyword"> Audience Manager</span> se realiza en <span class="keyword"> Adobe Media Optimizer</span>. </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p><a href="companies/admin-manage-company-destinations.md#manage-company-destinations"> Administrar destinos de la compañía</a> </p> </td> 
   <td colname="col2"> <p>Revisiones de menor importancia. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p><a href="companies/admin-amo-sync.md#concept_2B5537233DAA4860B3503B344F937D83"> Sincronización de ID con Media Optimizer</a> </p> </td> 
   <td colname="col2"> <p>Nueva documentación que describe la casilla de verificación de sincronización de AMO en cada contenedor de compañía. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p><a href="companies/admin-device-graph-options.md#concept_563615F1018340C683E0EE075F8F639D"> Opciones de gráfico de dispositivos para compañías</a> </p> </td> 
   <td colname="col2"> <p>Nueva documentación que describe cómo configurar las opciones de gráficos de dispositivos. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p><a href="admin-oauth2/aam-admin-api-requirements.md#concept_A7FAC9443CF34974A873E6B787616421"> Requisitos y recomendaciones de API</a> </p> </td> 
   <td colname="col2"> <p>Nueva documentación que describe algunos requisitos y recomendaciones que deben tenerse en cuenta y transmitirse a los clientes. Este contenido está duplicado en los documentos públicos con el mismo título y cambia en función de la audiencia que lea el contenido. Consulte <a href="https://experienceleague.adobe.com/docs/audience-manager/user-guide/api-and-sdk-code/rest-apis/aam-api-getting-started.html?lang=es#api-requirements-recommendations" format="https" scope="external"> Requisitos y recomendaciones de API</a> en los documentos públicos. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Actualizaciones de documentación de AAM 2016 {#aam-2016-docs-updates}

<table id="table_E9D9810EA8244B58A4F27D56CFE521FD"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Tema </th> 
   <th colname="col2" class="entry"> Descripción </th> 
  </tr>
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"><a href="admin-servers/create-ftp-server.md#task_BF1DD0E5ECA64AEC87EACABFCAEA2C6D"> Crear o editar un servidor FTP</a> </td> 
   <td colname="col2">Se ha añadido la dirección IP de FTP <b>52.44.29.204</b> de salida. </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p><a href="companies/admin-manage-company-destinations.md#manage-company-destinations"> Administrar destinos de la compañía</a> </p> </td> 
   <td colname="col2"> <p>Revisiones de menor importancia. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p><a href="admin-servers/create-http-server.md#task_5BF59581868E4144B965D644D36BEACD"> Crear o editar un servidor HTTP</a> </p> </td> 
   <td colname="col2"> <p>Se ha añadido la <b>Firma HTTP</b> en el Asistente para la creación de la configuración del servidor. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p><a href="admin-beta-environment.md#concept_4AA12E66F49A452C8BA4E91AA28060AA"> Entorno beta</a> </p> </td> 
   <td colname="col2"> <p>Se han actualizado las direcciones URL y los nombres de host del entorno beta. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p><a href="companies/outbound-active-user-filter.md#task_F5CF8BDDA5DB4D23837B59CADF7A623B"> Filtrar datos de salida solo por usuarios activos</a> </p> </td> 
   <td colname="col2"> <p>Instrucciones para generar un archivo de sincronización completo que incluya solo usuarios activos. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p><a href="formats/web-formats.md#reference_C392124A5F3F42E49F8AADDBA601ADFE"> Macros de formato HTTP</a> </p> </td> 
   <td colname="col2" morerows="1"> <p>Nueva documentación que enumera macros HTTP y ejemplos comunes. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p><a href="formats/web-format-examples.md#reference_98828E32B0964FF9AAC7C5400E88BA31"> Ejemplos de macros de formato HTTP</a> </p> </td> 
  </tr> 
 </tbody> 
</table>

## Actualizaciones de documentación de AAM 2015 {#aam-2015-docs-updates}

<table id="table_90F524BAAED44A45A1F6BF8BBA9F26F9"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Fecha y tema </th> 
   <th colname="col2" class="entry"> Descripción </th> 
  </tr>
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Diciembre de 2015 </p> <p><a href="formats/formats.md#concept_66AA2E78A25C4973B3230D5F75B192A2"> Formatos</a> </p> </td> 
   <td colname="col2"> <p>Se ha revisado la sección de macros y se han añadido ejemplos. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Actualizaciones de documentación de AAM 2014 {#aam-2014-docs-updates}

<table id="table_FA9962E19248418BA73D5A794A378C9D"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Fecha y tema </th> 
   <th colname="col2" class="entry"> Descripción </th> 
  </tr>
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>12 de noviembre de 2014 </p> <p> <a href="formats/formats.md#concept_66AA2E78A25C4973B3230D5F75B192A2"> Formatos</a> </p> </td> 
   <td colname="col2"> <p>Se ha añadido información sobre la macro &lt;MCID&gt;. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>23 de octubre de 2014 </p> <p><a href="formats/admin-create-format.md#task_1A51FC9189DB439FB218D91F3875FD67"> Crear o editar un formato</a> </p> </td> 
   <td colname="col2"> <p>Se ha añadido información sobre la opción <span class="wintitle"> .info Receipt</span>. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>23 de octubre de 2014 </p> <p><a href="formats/formats.md#concept_66AA2E78A25C4973B3230D5F75B192A2"> Formatos</a> </p> </td> 
   <td colname="col2"> <p>Nueva página. Tenga en cuenta que esta página es un trabajo en curso y se actualizará en los próximos días. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>22 de octubre de 2014 </p> <p><a href="admin-destination-troubleshooting.md#"> Solución de problemas de configuración de destino</a> </p> </td> 
   <td colname="col2"> <p>Nuevo tema. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>21 de octubre de 2014 </p> <p><a href="companies/admin-manage-company-destinations.md#manage-company-destinations"> Administrar destinos de la compañía</a> </p> </td> 
   <td colname="col2"> <p>Se ha reescrito el tema entero. Se ha añadido información y configuración adicional. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>25 de septiembre de 2014 </p> <p><a href="companies/admin-manage-company-profiles.md"> Crear una compañía</a> </p> </td> 
   <td colname="col2"> <p>Se ha añadido información adicional en las secciones <span class="wintitle"> Ciclo de vida</span> y <span class="wintitle"> Tipos de cuenta</span>. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>25 de septiembre de 2014 </p> <p><a href="companies/admin-manage-company-profiles.md#edit-company-profile"> Editar un perfil de compañía</a> </p> </td> 
   <td colname="col2"> <p>Se ha añadido información adicional en las secciones <span class="wintitle"> Ciclo de vida</span> y <span class="wintitle"> Tipos de cuenta</span>. </p> </td> 
  </tr> 
 </tbody> 
</table>
