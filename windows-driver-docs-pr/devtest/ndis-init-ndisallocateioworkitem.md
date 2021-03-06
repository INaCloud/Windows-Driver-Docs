---
title: Init\_NdisAllocateIoWorkItem rule (ndis)
description: The Init\_NdisAllocateIoWorkItem rule specifies that if NdisAllocateIoWorkItem is called at least once during MiniportInitializeEx, the NdisFreeIoWorkItem function should - be called at least once in MPHaltEx, if MiniportInitializeEx succeeds.
ms.assetid: B7889948-741C-4C54-B27F-3175ED4EA7BA
ms.author: windowsdriverdev
ms.date: 05/21/2018
ms.topic: article
ms.prod: windows-hardware
ms.technology: windows-devices
keywords: ["Init_NdisAllocateIoWorkItem rule (ndis)"]
topic_type:
- apiref
api_name:
- Init_NdisAllocateIoWorkItem
api_type:
- NA
ms.localizationpriority: medium
---

# Init\_NdisAllocateIoWorkItem rule (ndis)


The **Init\_NdisAllocateIoWorkItem** rule specifies that if [**NdisAllocateIoWorkItem**](https://msdn.microsoft.com/library/windows/hardware/ff561604) is called at least once during [*MiniportInitializeEx*](https://msdn.microsoft.com/library/windows/hardware/ff559389), the [**NdisFreeIoWorkItem**](https://msdn.microsoft.com/library/windows/hardware/ff561855) function should:

-   - be called at least once in MPHaltEx, if [*MiniportInitializeEx*](https://msdn.microsoft.com/library/windows/hardware/ff559389) succeeds.
-   - be called in [*MiniportInitializeEx*](https://msdn.microsoft.com/library/windows/hardware/ff559389), if *MiniportInitializeEx* fails.

|              |      |
|--------------|------|
| Driver model | NDIS |

How to test
-----------

<table>
<colgroup>
<col width="100%" />
</colgroup>
<thead>
<tr class="header">
<th align="left">At compile time</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td align="left"><p>Run [Static Driver Verifier](https://msdn.microsoft.com/library/windows/hardware/ff552808) and specify the <strong>Init_NdisAllocateIoWorkItem</strong> rule.</p>
Use the following steps to run an analysis of your code:
<ol>
<li>[Prepare your code (use role type declarations).](https://msdn.microsoft.com/library/windows/hardware/hh454281#preparing-your-source-code)</li>
<li>[Run Static Driver Verifier.](https://msdn.microsoft.com/library/windows/hardware/hh454281#running-static-driver-verifier)</li>
<li>[View and analyze the results.](https://msdn.microsoft.com/library/windows/hardware/hh454281#viewing-and-analyzing-the-results)</li>
</ol>
<p>For more information, see [Using Static Driver Verifier to Find Defects in Drivers](https://msdn.microsoft.com/library/windows/hardware/hh454281).</p></td>
</tr>
</tbody>
</table>

Applies to
----------

[**NdisAllocateIoWorkItem**](https://msdn.microsoft.com/library/windows/hardware/ff561604)
[**NdisFreeIoWorkItem**](https://msdn.microsoft.com/library/windows/hardware/ff561855)
[**RemoveHeadList**](https://msdn.microsoft.com/library/windows/hardware/ff561032)
 

 





