﻿---
title: ReleaseUpdateTransformDB50_Vend.vendInvoiceInfoLinePreUpgradeProcess Upgrade Script
TOCTitle: ReleaseUpdateTransformDB50_Vend.vendInvoiceInfoLinePreUpgradeProcess Upgrade Script
ms:assetid: 194153cc-cc56-6f79-fa5f-1195c5e0dd7a
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/JJ718630(v=AX.60)
ms:contentKeyID: 49706913
ms.date: 05/18/2015
mtps_version: v=AX.60
---

# ReleaseUpdateTransformDB50\_Vend.vendInvoiceInfoLinePreUpgradeProcess Upgrade Script 


_**Applies To:** Microsoft Dynamics AX 2012 R3, Microsoft Dynamics AX 2012 R2, Microsoft Dynamics AX 2012 Feature Pack, Microsoft Dynamics AX 2012_

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><strong>Class</strong></p></td>
<td><p>ReleaseUpdateTransformDB50_Vend</p></td>
</tr>
<tr class="even">
<td><p><strong>Method</strong></p></td>
<td><p>vendInvoiceInfoLinePreUpgradeProcess</p></td>
</tr>
<tr class="odd">
<td><p><strong>Description</strong></p></td>
<td><p>Creates data in the SourceDocumentLine table, initializes the SourceDocumentLine, TaxGroup, and TaxItemGroup fields in the VendInvoiceInfoLine table.</p></td>
</tr>
<tr class="even">
<td><p><strong>Script Type</strong></p></td>
<td><p>Preprocessing 60: Live</p></td>
</tr>
<tr class="odd">
<td><p><strong>Microsoft Dynamics AX Source</strong></p></td>
<td><p>Microsoft Dynamics AX 4.0</p>
<p>Microsoft Dynamics AX 2009</p></td>
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
<td><p>Accounts payable</p></td>
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
<td><p>VendInvoiceInfoLine</p></td>
</tr>
<tr class="even">
<td><p>SourceDocumentLine</p></td>
</tr>
</tbody>
</table>


## Remarks

This upgrade is required in order to create records in the SourceDocumentLine table which is a mandatory FK to the VendInvoiceInfoLine table in the next release.

## Data Migration Section

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th><p>From Table: PurchLine</p></th>
<th><p>To Table: VendInvoiceInfoLine</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>TaxGroup</p></td>
<td><p>TaxGroup</p></td>
</tr>
<tr class="even">
<td><p>TaxItemGroup</p></td>
<td><p>TaxItemGroup</p></td>
</tr>
</tbody>
</table>


<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th><p>From Table: SourceDocumentLine</p></th>
<th><p>To Table: VendInvoiceInfoLine</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>RecId</p></td>
<td><p>SourceDocumentLine</p></td>
</tr>
</tbody>
</table>


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
<td><p>SourceDocumentLine</p></td>
<td><p></p></td>
<td><p></p></td>
</tr>
<tr class="even">
<td><p>VendInvoiceInfoLine</p></td>
<td><p>TaxGroup</p></td>
<td><p>TaxGroup</p></td>
</tr>
<tr class="odd">
<td><p>VendInvoiceInfoLine</p></td>
<td><p>TaxItemGroup</p></td>
<td><p>TaxItemGroup</p></td>
</tr>
</tbody>
</table>

  


