---
title: KSPROPERTY\_VPCONFIG\_GETCONNECTINFO
description: The KSPROPERTY\_VPCONFIG\_GETCONNECTINFO property retrieves all possible video port configurations.
ms.assetid: 30ac1f7d-0218-49ed-8f6d-e58f56aee70e
keywords: ["KSPROPERTY_VPCONFIG_GETCONNECTINFO Streaming Media Devices"]
topic_type:
- apiref
api_name:
- KSPROPERTY_VPCONFIG_GETCONNECTINFO
api_location:
- ksmedia.h
api_type:
- HeaderDef
ms.author: windowsdriverdev
ms.date: 11/28/2017
ms.topic: article
ms.prod: windows-hardware
ms.technology: windows-devices
ms.localizationpriority: medium
---

# KSPROPERTY\_VPCONFIG\_GETCONNECTINFO


The KSPROPERTY\_VPCONFIG\_GETCONNECTINFO property retrieves all possible video port configurations.

## <span id="ddk_ksproperty_vpconfig_getconnectinfo_ks"></span><span id="DDK_KSPROPERTY_VPCONFIG_GETCONNECTINFO_KS"></span>


### Usage Summary Table

<table>
<colgroup>
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
</colgroup>
<thead>
<tr class="header">
<th>Get</th>
<th>Set</th>
<th>Target</th>
<th>Property descriptor type</th>
<th>Property value type</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>Yes</p></td>
<td><p>No</p></td>
<td><p>Pin</p></td>
<td><p>[<strong>KSPROPERTY</strong>](https://docs.microsoft.com/windows-hardware/drivers/ddi/content/ks/ns-ks-ksidentifier)</p></td>
<td><p>[<strong>DDVIDEOPORTCONNECT</strong>](https://msdn.microsoft.com/library/windows/hardware/ff550388)</p></td>
</tr>
</tbody>
</table>

 

The property value (operation data) is a DDVIDEOPORTCONNECT structure that describes the configuration of a video port connection.

Requirements
------------

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p>Header</p></td>
<td>Ksmedia.h (include Ksmedia.h)</td>
</tr>
</tbody>
</table>

## See also


[**DDVIDEOPORTCONNECT**](https://msdn.microsoft.com/library/windows/hardware/ff550388)

 

 






