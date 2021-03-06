﻿---
title: ReleaseUpdateDB60_Ledger.allowNoDupLedgerAccountRestriction_CNAcc Upgrade Script
TOCTitle: ReleaseUpdateDB60_Ledger.allowNoDupLedgerAccountRestriction_CNAcc Upgrade Script
ms:assetid: ccd0093a-81ff-9d54-a56a-07616d450c41
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/JJ719707(v=AX.60)
ms:contentKeyID: 49711273
ms.date: 05/18/2015
mtps_version: v=AX.60
---

# ReleaseUpdateDB60\_Ledger.allowNoDupLedgerAccountRestriction\_CNAcc Upgrade Script 


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
<td><p>allowNoDupLedgerAccountRestriction_CNAcc</p></td>
</tr>
<tr class="odd">
<td><p><strong>Description</strong></p></td>
<td><p>Updates the AccountRestrictionIdx index in the LedgerAccountRestriction_CN table to not allow duplicate records.</p></td>
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
<td><p>LEDGERACCOUNTRESTRICTION_CN</p></td>
</tr>
</tbody>
</table>


## Remarks

After updating the LedgerAccountRestriction\_CN surrogate key field with the value of the RecId field of the LedgerAccountRestriction\_CN table, the AccountRestrictionIdx index is reset to not allow duplicate records.

  


