﻿---
title: ReleaseUpdateTransformDB41_Prod.validateWrkCtrTableGroupSameInventLoc Upgrade Script
TOCTitle: ReleaseUpdateTransformDB41_Prod.validateWrkCtrTableGroupSameInventLoc Upgrade Script
ms:assetid: 6d04410e-1634-bd07-1074-b948c9d612d4
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/JJ685717(v=AX.60)
ms:contentKeyID: 49708918
ms.date: 05/18/2015
mtps_version: v=AX.60
---

# ReleaseUpdateTransformDB41\_Prod.validateWrkCtrTableGroupSameInventLoc Upgrade Script 


_**Applies To:** Microsoft Dynamics AX 2012 R3, Microsoft Dynamics AX 2012 R2, Microsoft Dynamics AX 2012 Feature Pack, Microsoft Dynamics AX 2012_

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><strong>Class</strong></p></td>
<td><p>ReleaseUpdateTransformDB41_Prod</p></td>
</tr>
<tr class="even">
<td><p><strong>Method</strong></p></td>
<td><p>validateWrkCtrTableGroupSameInventLoc</p></td>
</tr>
<tr class="odd">
<td><p><strong>Description</strong></p></td>
<td><p>Validates if work centers have the same warehouse as the work center group.</p></td>
</tr>
<tr class="even">
<td><p><strong>Script Type</strong></p></td>
<td><p>Upgrade readiness scripts</p></td>
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
<td><p>Production</p></td>
</tr>
</tbody>
</table>


<table xmlns="http://www.w3.org/1999/xhtml">
              <tr><th colspan="2">
		
   <p>
   
	 Validation Issues
  </p>
  </th></tr>
              <tr><td>
		
   <p>
   
	 
            Validation Issues Description
          
  </p>
  </td><td>
		
   <p>
   
	 Validates that the warehouse on the work center doesn’t differ from the warehouse on the corresponding work center group. All work centers in a work center group must have the same warehouse as the work center group.
  </p>
  </td></tr>
              <tr><td>
		
   <p>
   
	 
            Checked Conditions
          
  </p>
  </td><td>
		
   <p>
   
	 Checks whether there are work centers with warehouses that differ from the warehouse of the work center group.
  </p>
  </td></tr>
              <tr><td>
		
   <p>
   
	 
            Mitigation/How-to-fix
          
  </p>
  </td><td>
		
   <p>
   
	 Change the warehouse of the work center or the work center group.
  </p>
  </td></tr>
            </table>

  


