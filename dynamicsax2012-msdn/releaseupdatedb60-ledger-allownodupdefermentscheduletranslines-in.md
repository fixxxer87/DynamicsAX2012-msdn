﻿---
title: ReleaseUpdateDB60_Ledger.allowNoDupDefermentScheduleTransLines_IN
TOCTitle: ReleaseUpdateDB60_Ledger.allowNoDupDefermentScheduleTransLines_IN
ms:assetid: 30c97c9d-43c3-d791-9fb8-e264b5459464
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/JJ736071(v=AX.60)
ms:contentKeyID: 49707485
ms.date: 05/18/2015
mtps_version: v=AX.60
---

# ReleaseUpdateDB60\_Ledger.allowNoDupDefermentScheduleTransLines\_IN 


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
<td><p>allowNoDupDefermentScheduleTransLines_IN</p></td>
</tr>
<tr class="odd">
<td><p><strong>Description</strong></p></td>
<td><p>Updates the index &lt;c&gt;ExtDueDatePeriodIdx&lt;/c&gt; in the table &lt;c&gt;DefermentScheduleTransLines_IN&lt;/c&gt; not to allow duplicate records.</p></td>
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
<td><p>DEFERMENTSCHEDULETRANSLINES_IN</p></td>
</tr>
</tbody>
</table>


## Remarks

ExtDueDatePeriodIdx is reset not to allow duplicate records.

  


