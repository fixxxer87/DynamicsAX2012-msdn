﻿---
title: ReleaseUpdateTransformDB40_Bank.bankDepositPreUpgradeProcess Upgrade Script
TOCTitle: ReleaseUpdateTransformDB40_Bank.bankDepositPreUpgradeProcess Upgrade Script
ms:assetid: c6d31d7f-e1b4-fae8-183b-014fb47faf16
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/JJ719569(v=AX.60)
ms:contentKeyID: 49711136
ms.date: 05/18/2015
mtps_version: v=AX.60
---

# ReleaseUpdateTransformDB40\_Bank.bankDepositPreUpgradeProcess Upgrade Script 


_**Applies To:** Microsoft Dynamics AX 2012 R3, Microsoft Dynamics AX 2012 R2, Microsoft Dynamics AX 2012 Feature Pack, Microsoft Dynamics AX 2012_

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><strong>Class</strong></p></td>
<td><p>ReleaseUpdateTransformDB40_Bank</p></td>
</tr>
<tr class="even">
<td><p><strong>Method</strong></p></td>
<td><p>bankDepositPreUpgradeProcess</p></td>
</tr>
<tr class="odd">
<td><p><strong>Description</strong></p></td>
<td><p>Transforms data from the LedgerAccountNum field to the LedgerDimension field in the BankDeposit table.</p></td>
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
<td><p>Bank</p></td>
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
<td><p>BankDeposit</p></td>
</tr>
</tbody>
</table>


## Remarks

This upgrade is required in order to convert account and dimension data to the new accounts and dimension model for Microsoft Dynamics AX 2012.

## Data Migration Section

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th><p>From Table: BankDeposit</p></th>
<th><p>To Table: Shadow_BankDeposit</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>LedgerAccountNum</p></td>
<td><p>LedgerDimension</p></td>
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
<td><p>BankDeposit</p></td>
<td><p>LedgerDimension</p></td>
<td><p>LedgerDimensionDefaultAccount</p></td>
</tr>
</tbody>
</table>


## Deleted Tables or Fields

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th><p>Table</p></th>
<th><p>Field</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>BankDeposit</p></td>
<td><p>LedgerAccountNum</p></td>
</tr>
</tbody>
</table>

  


