---
description: Enumera las macros que puede utilizar para crear archivos de datos basados en FTP. Algunas macros se pueden utilizar para todos los campos y filas del archivo de datos. Otras macros son específicas del encabezado y de las filas de datos únicamente.
seo-description: Lists the macros you can use to create FTP-based data files. Some macros can be used for all data file fields and rows. Other macros are specific to header and data rows only.
seo-title: File Format Macros
title: Macros de formato de archivo
uuid: f91c91b6-6581-4ed7-8d7f-f8532bd41df9
exl-id: e686bc33-da3e-49a9-8c71-2bc6ca399bfb
TQID: https://experienceleague.adobe.com/ATzqYmfRIVDeQ3DZpbcZkCP4Jjsapw9Nfyli1QFR8-o
product_v2:
  - id: df80eeb1-8d72-467e-b0df-9d51c7d3a0a1
source-git-commit: d2bed13a6ac7d38ae79b65d492b6de0ca6b6d488
workflow-type: tm+mt
source-wordcount: 686
ht-degree: 1%

---

# Macros de formato de archivo {#file-format-macros}

Enumera las macros que puede utilizar para crear archivos de datos basados en [!DNL FTP]. Algunas macros se pueden utilizar para todos los campos y filas del archivo de datos. Otras macros son específicas del encabezado y de las filas de datos únicamente.

## Macros comunes {#common-macros}

Estas macros se pueden utilizar en cualquier campo de formato. Para ver ejemplos, vea [Ejemplos de macros de formato de archivo](../formats/file-format-examples.md).

<table id="table_A3309E175ABF4651BD11CE3632B3C553"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Macro </th> 
   <th colname="col2" class="entry"> Descripción </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p> <code>ASCII_SOH</code> </p> </td> 
   <td colname="col2"> <p>Un carácter ASCII no imprimible. Indica el inicio de una fila o una sección de contenido. También se puede utilizar para separar columnas de datos en un archivo. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>DPID</code> </p> </td> 
   <td colname="col2"> <p>ID del proveedor de datos de destino. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>MASTER_DPID</code> </p> </td> 
   <td colname="col2"> <p>ID de usuario ID de proveedor de datos clave. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>ORDER_ID</code> </p> </td> 
   <td colname="col2"> <p>ID de pedido/destino. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>PIDALIAS</code> </p> </td> 
   <td colname="col2"> <p>Un alias para un ID de pedido/destino. </p> <p>El valor de este alias se establece en el campo <span class="wintitle"> Id. de cuenta externa </span> para un destino (en la sección <span class="wintitle"> Configuración básica </span>). </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>SYNC_MODE</code> </p> </td> 
   <td colname="col2"> <p>Indica el tipo de sincronización. Acepta las siguientes variables opcionales: </p> 
    <ul id="ul_87E8E3CE6565447A9810B5119298CC7B"> 
     <li id="li_66F4889FB84E40AC92F69F3FF6B0042C"> <code>full</code>: sincronización completa. </li> 
     <li id="li_BFE2C2D9A33A44FB9A840A7232ECCFFF"> <code>iter</code>: sincronización incremental. </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>SYNC_TYPE</code> </p> </td> 
   <td colname="col2"> <p>Indica el método de transferencia de datos. Acepta las siguientes variables opcionales: </p> 
    <ul id="ul_13BE35BBBF7C4C67AEFC514C5D192902"> 
     <li id="li_195FE9B4C5494600BD17D7172A8FB630"> <code>ftp</code> </li> 
     <li id="li_751AD59C4C934D66BC530D9806B500AF"> <code>http</code> </li> 
     <li id="li_4638AF7D1FB54E2C890045048B85309C"> <code>s3</code> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>TIMESTAMP</code> </p> </td> 
   <td colname="col2"> <p>Una marca de tiempo Unix, UTC y de 10 dígitos. </p> <p>También se le puede aplicar el formato <code>YYYYMMDDhhmmss</code> según las reglas de formato de fecha y hora de Java. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Macros de campo de encabezado {#header-field-macros}

Macros utilizadas solo en campos de encabezado. Para ver ejemplos, vea [Ejemplos de macros de formato de archivo](../formats/file-format-examples.md).

<table id="table_1A8BD1750F4940B3A34E3F80371A447A"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Macro </th> 
   <th colname="col2" class="entry"> Descripción </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p> <code>TAB</code> </p> </td> 
   <td colname="col2"> <p>Utilizada como separador, esta macro inserta una tabulación entre los campos. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Macros de fila de datos {#data-row-macros}

Macros utilizadas solo en filas de datos. Para ver ejemplos, vea [Ejemplos de macros de formato de archivo](../formats/file-format-examples.md).

<table id="table_E378F94A3907407AA8110C8EE6C10909"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Macro </th> 
   <th colname="col2" class="entry"> Descripción </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p> <code>CLOSE_CURLY_BRACKET</code> </p> </td> 
   <td colname="col2"> <p>Inserta un carácter de llave cerrada <code>&rbrace;</code>. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>COMMA</code> </p> </td> 
   <td colname="col2"> <p>Inserta una coma. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>DP_UUID</code> </p> </td> 
   <td colname="col2"> <p> <span class="term"> Identificador De Usuario Único Del Socio De Datos </span>. Devuelve el identificador que asignó a un usuario o visitante del sitio si ese identificador ya se ha sincronizado con un identificador de dispositivo <span class="keyword"> Audience Manager </span>. </p> <p>Si el DPID es 0, esta macro devolverá el ID <span class="keyword"> de Audience Manager </span> en lugar del ID del usuario. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>DP_UUID_LIST</code> </p> </td> 
   <td colname="col2"> <p>Devuelve una lista que contiene varios ID de un socio de datos. Esto resulta útil si tiene una organización grande con varias subdivisiones u otros grupos organizativos con los que puede compartir datos. Esta macro devuelve una lista de los identificadores de esos grupos subordinados. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>DPUUIDS</code> </p> </td> 
   <td colname="col2"> <p>El resultado de esta macro asigna el ID del proveedor de datos (DPID) a los ID de usuario únicos relacionados (DPUUID). Esta macro debe tener una cadena de formato para controlar su resultado. El resultado de la muestra sería similar al siguiente: </p> <p> <code>"dpids=dpid1,dpid2,...dpid n|maxMappings= n|format=json"</code> </p> <p>La configuración <code>maxMappings</code> determina cuántas asignaciones desea que devuelva la macro. Cuando <code>maxMappings=0</code>, esta macro devuelve todas las asignaciones para cada DPID especificado. Los datos se ordenan por marca de tiempo (más reciente primero) y devuelve los resultados con la marca de tiempo más grande primero. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>endif</code> </p> </td> 
   <td colname="col2"> <p>Requerido al usar las macros condicionales <code>if</code> y <code>SEGMENT_LIST</code> y <code>REMOVED_SEGMENT_LIST</code>. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>if(SEGMENT_LIST &amp;&amp; REMOVED_SEGMENT_LIST)endif</code> </p> </td> 
   <td colname="col2"> <p>Esta combinación de macros crea una declaración condicional que enumera los segmentos a los que pertenecen los usuarios de <i> y de los que se han eliminado </i>. Devuelve una cadena vacía si no se cumplen ambas condiciones o si no hay datos. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>MCID</code> </p> </td> 
   <td colname="col2"> <p> <span class="keyword"> ID. </span> de Adobe Experience Cloud. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>OPEN_CURLY_BRACKET</code> </p> </td> 
   <td colname="col2"> <p>Inserta un carácter de llave <code>&lbrace;</code> abierto. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>OPT_OUT</code> </p> </td> 
   <td colname="col2"> <p>Obsoleta. No utilice. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>OUTPUT_ATTRIBUTE_TYPE</code> </p> </td> 
   <td colname="col2"> <p>Obsoleta. No utilice. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>OUTPUT_ATTRIBUTE_VALUE</code> </p> </td> 
   <td colname="col2"> <p>Devuelve <code>1</code> como un valor estático codificado. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>PID</code> </p> </td> 
   <td colname="col2"> <p>ID de socio (PID). El PID aparece en la ficha </span> del perfil <span class="wintitle"> en la interfaz de usuario de administración. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>REMOVED_SEGMENT_LIST</code> </p> </td> 
   <td colname="col2"> <p>Devuelve una lista de los segmentos que se han eliminado, si los hay. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>SEGMENT_LIST</code> </p> </td> 
   <td colname="col2"> <p>Devuelve una lista de segmentos de una lista. Acepta las siguientes variables opcionales: </p> 
    <ul id="ul_B111AA0D6C18445598A1444B8B7E9325"> 
     <li id="li_8603B40229624856AF1FBC434DB8F16A"> <code>segmentId</code>: ID heredado. Obsoleta. Usar <code>sid</code> (solo minúsculas). </li> 
     <li id="li_1EF40DDCA3C5447586904CF021D8F912"> <code>csegid</code>: ID heredado. Obsoleta. Usar <code>sid</code> (solo minúsculas). </li> 
     <li id="li_D85F0A5D16AE4DAFB55C17DBB35EA66E"> <code>sid</code>: ID de segmento. </li> 
     <li id="li_9BE103EFD8384464B46FAC00422431DB"> <code>type</code>: devuelve <code>5</code>, un valor estático codificado que identifica los datos como datos de segmento. </li> 
     <li id="li_FE5049089F2944FA9DB9F9D546DBA167"> <code>alias</code>: asignación del segmento. Obsoleta. Usar <code>sid</code> (solo minúsculas). </li> 
     <li id="li_DD778AA2D1DB4D409CF5026B5D9DBD27"> <code>lastUpdateTime</code>: una marca de tiempo Unix que indica la última vez que se realizó un segmento. </li> 
    </ul> <p>Coloque estas variables entre llaves después de la macro. Por ejemplo, este código separa los resultados con una barra vertical "|": <code>&lt;SEGMENT_LIST:{seg|&lt;seg.type&gt;,&lt;seg.sid&gt;}; separator="|"&gt;</code> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>SET_ATTRIBUTES</code> </p> </td> 
   <td colname="col2"> <p>Devuelve <code>1</code> como un valor estático codificado. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>TAB</code> </p> </td> 
   <td colname="col2"> <p>Inserta un separador de tabulaciones. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>TRAIT_LIST</code> </p> </td> 
   <td colname="col2"> <p>Devuelve una lista de características. Acepta los siguientes argumentos opcionales: </p> 
    <ul id="ul_757DEB56E4F849768468F3C166B0D171"> 
     <li id="li_859E1F4F21D645519F150DC512B3EB1A"> <code>type</code>: tipos de rasgos identificados por un identificador numérico. Esta variable devuelve: 
      <ul id="ul_C9839266783D42CCADAAC3FEA33BE4D7"> 
       <li id="li_6996A218E3F04EC3BC70032559DD87FC"> <code>10</code> que identifica un rasgo de DPM (sin conexión, incorporado por un trabajo entrante). </li> 
       <li id="li_831FF929BF50434C8804C13E5786DF79"> <code>3</code> que identifica un rasgo basado en reglas (en tiempo real,; incorporado a través de <span class="wintitle"> DCS </span>). </li> 
      </ul> </li> 
     <li id="li_E84D6BC80AEE4F10963C9882C4151ED4"> <code>traitId</code>: ID de rasgo. </li> 
     <li id="li_D30A849BA35248E6B9110FA3ADEFC332"> <code>lastRealized</code>: última vez que se realizó el rasgo. Marca de tiempo Unix. </li> 
    </ul> <p>Coloque estas variables entre llaves después de la macro. Por ejemplo, este código separa los resultados con una barra vertical "|": <code>TRAIT_LIST{type|traitId};separator="|"</code> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <code>UUID</code> </p> </td> 
   <td colname="col2"> <p> <span class="keyword"> ID de usuario </span> de Audience Manager. </p> </td> 
  </tr> 
 </tbody> 
</table>
