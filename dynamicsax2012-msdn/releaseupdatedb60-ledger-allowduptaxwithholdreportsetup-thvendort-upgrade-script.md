﻿---
title: ReleaseUpdateDB60_Ledger.allowDupTaxWithholdReportSetup_THVendorT Upgrade Script
TOCTitle: ReleaseUpdateDB60_Ledger.allowDupTaxWithholdReportSetup_THVendorT Upgrade Script
ms:assetid: 3d2de1ae-4daa-7468-1260-66191543b175
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/JJ718730(v=AX.60)
ms:contentKeyID: 49707775
ms.date: 05/18/2015
mtps_version: v=AX.60
---

# ReleaseUpdateDB60\_Ledger.allowDupTaxWithholdReportSetup\_THVendorT Upgrade Script 


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
<td><p>allowDupTaxWithholdReportSetup_THVendorT</p></td>
</tr>
<tr class="odd">
<td><p><strong>Description</strong></p></td>
<td><p>Updates the VendorTypeItemGroupIdx index in the TaxWithholdReportSetup_TH table to allow for duplicate records.</p></td>
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
<td><p>TaxWithholdReportSetup_TH</p></td>
</tr>
</tbody>
</table>


## Remarks

The TaxWithholdItemGroup field is replaced with the new TaxWithholdItemGroupHeading\_TH surrogate key field in the unique VendorTypeItemGroupIdx index. Initially, this field contains no value. Therefore, the index is set to allow for duplicate values before the field is updated with the value of the RecId field of the TaxWithholdItemGroupHeading\_TH table.

  


