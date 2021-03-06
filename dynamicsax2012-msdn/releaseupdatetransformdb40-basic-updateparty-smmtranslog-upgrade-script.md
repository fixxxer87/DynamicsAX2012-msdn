﻿---
title: ReleaseUpdateTransformDB40_Basic.updateParty_smmTransLog Upgrade Script
TOCTitle: ReleaseUpdateTransformDB40_Basic.updateParty_smmTransLog Upgrade Script
ms:assetid: 79e5971f-7d1b-da26-7718-0312f1ad5f5d
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/JJ719400(v=AX.60)
ms:contentKeyID: 49709191
ms.date: 05/18/2015
mtps_version: v=AX.60
---

# ReleaseUpdateTransformDB40\_Basic.updateParty\_smmTransLog Upgrade Script 


_**Applies To:** Microsoft Dynamics AX 2012 R3, Microsoft Dynamics AX 2012 R2, Microsoft Dynamics AX 2012 Feature Pack, Microsoft Dynamics AX 2012_

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><strong>Class</strong></p></td>
<td><p>ReleaseUpdateTransformDB40_Basic</p></td>
</tr>
<tr class="even">
<td><p><strong>Method</strong></p></td>
<td><p>updateParty_smmTransLog</p></td>
</tr>
<tr class="odd">
<td><p><strong>Description</strong></p></td>
<td><p>Updates the Party field in the smmTransLog table.</p></td>
</tr>
<tr class="even">
<td><p><strong>Script Type</strong></p></td>
<td><p>Preprocessing 60: Live</p></td>
</tr>
<tr class="odd">
<td><p><strong>Microsoft Dynamics AX Source</strong></p></td>
<td><p>Microsoft Dynamics AX 4.0</p></td>
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
<td><p>CRM</p></td>
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
<td><p>smmTransLog</p></td>
</tr>
</tbody>
</table>


## Remarks

This upgrade is required in order to update the new party field in the smmTransLog table. The party will be kept as a reference to the DirPartyTable record.

## New Tables or Fields

<table>
<colgroup>
<col style="width: 33%" />
<col style="width: 33%" />
<col style="width: 33%" />
</colgroup>
<thead>
<tr class="header">
<th><p>Table</p></th>
<th><p>Field</p></th>
<th><p>Extended Data Type</p>
<p>-or- Base Enum</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>smmTransLog</p></td>
<td><p>Party</p></td>
<td><p></p></td>
</tr>
</tbody>
</table>

  


