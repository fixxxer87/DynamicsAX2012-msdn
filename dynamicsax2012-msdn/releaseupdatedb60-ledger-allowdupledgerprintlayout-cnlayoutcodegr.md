﻿---
title: ReleaseUpdateDB60_Ledger.allowDupLedgerPrintLayout_CNLayoutCodeGr
TOCTitle: ReleaseUpdateDB60_Ledger.allowDupLedgerPrintLayout_CNLayoutCodeGr
ms:assetid: 828f93e6-8f4d-1d41-79a0-5f02e9c45f06
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/JJ685951(v=AX.60)
ms:contentKeyID: 49709403
ms.date: 05/18/2015
mtps_version: v=AX.60
---

# ReleaseUpdateDB60\_Ledger.allowDupLedgerPrintLayout\_CNLayoutCodeGr 


_**Applies To:** Microsoft Dynamics AX 2012 R3, Microsoft Dynamics AX 2012 R2_

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><strong>Class</strong></p></td>
<td><p>ReleaseUpdateDB60_Ledger</p></td>
</tr>
<tr class="even">
<td><p><strong>Method</strong></p></td>
<td><p>allowDupLedgerPrintLayout_CNLayoutCodeGr</p></td>
</tr>
<tr class="odd">
<td><p><strong>Description</strong></p></td>
<td><p>Updates the index &lt;c&gt;LayoutCodeGroupIdx&lt;/c&gt; in the table &lt;c&gt;LedgerPrintLayout_CN&lt;/c&gt; not to allow duplicate records.</p></td>
</tr>
</tbody>
</table>


## Affected Modules and Tables

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><p>Affected Modules</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>General ledger</p></td>
</tr>
</tbody>
</table>


<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><p>Affected Tables</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>LEDGERPRINTLAYOUT_CN</p></td>
</tr>
</tbody>
</table>


## Remarks

After updating the surrogate key field LedgerPrintLayout\_CN with the value of the RecId field of the table LedgerPrintLayout\_CN, the index LayoutCodeIdx is reset not to allow duplicate records.

  


