﻿---
title: ReleaseUpdateDB60_Ledger.allowDupEximSionTable_IN Upgrade Script
TOCTitle: ReleaseUpdateDB60_Ledger.allowDupEximSionTable_IN Upgrade Script
ms:assetid: 753a12d6-e17e-1114-ec48-f13854b52419
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/JJ719310(v=AX.60)
ms:contentKeyID: 49709102
ms.date: 05/18/2015
mtps_version: v=AX.60
---

# ReleaseUpdateDB60\_Ledger.allowDupEximSionTable\_IN Upgrade Script 


_**Applies To:** Microsoft Dynamics AX 2012 R3, Microsoft Dynamics AX 2012 R2, Microsoft Dynamics AX 2012 Feature Pack, Microsoft Dynamics AX 2012_

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
<td><p>allowDupEximSionTable_IN</p></td>
</tr>
<tr class="odd">
<td><p><strong>Description</strong></p></td>
<td><p>Updates the ProductGroupValidFromValidToIdx index in the EximSionTable_IN table to allow for duplicate records.</p></td>
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
<td><p>Ledger</p></td>
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
<td><p>EximSionTable_IN</p></td>
</tr>
</tbody>
</table>


## Remarks

The ProductGroup field is replaced with the new EximProductGroupTable surrogate key field along with the date effectivity fields in the new ProductGroupValidFromToIdx unique index. Initially the EximProductGroupTable, ValidFrom, and ValidTo fields contains no value. So the index is set to allow for duplicates before the field is updated with the value of the record ID fields of the EximProductGroupTable\_IN unique index.

  


