---
UID: NF:dvbsiparser.IDVB_SDT.GetRecordRunningStatus
title: IDVB_SDT::GetRecordRunningStatus (dvbsiparser.h)
description: This topic applies to Update Rollup 2 for Microsoft Windows XP Media Center Edition 2005 and later.helpviewer_keywords: ["GetRecordRunningStatus","GetRecordRunningStatus method [Microsoft TV Technologies]","GetRecordRunningStatus method [Microsoft TV Technologies]","IDVB_SDT interface","IDVB_SDT interface [Microsoft TV Technologies]","GetRecordRunningStatus method","IDVB_SDT.GetRecordRunningStatus","IDVB_SDT::GetRecordRunningStatus","IDVB_SDTGetRecordRunningStatus","dvbsiparser/IDVB_SDT::GetRecordRunningStatus","mstv.idvb_sdt_getrecordrunningstatus"]
old-location: mstv\idvb_sdt_getrecordrunningstatus.htm
tech.root: mstv
ms.assetid: a6e799b3-f90e-415f-a380-e90d69184fe2
ms.date: 12/05/2018
ms.keywords: GetRecordRunningStatus, GetRecordRunningStatus method [Microsoft TV Technologies], GetRecordRunningStatus method [Microsoft TV Technologies],IDVB_SDT interface, IDVB_SDT interface [Microsoft TV Technologies],GetRecordRunningStatus method, IDVB_SDT.GetRecordRunningStatus, IDVB_SDT::GetRecordRunningStatus, IDVB_SDTGetRecordRunningStatus, dvbsiparser/IDVB_SDT::GetRecordRunningStatus, mstv.idvb_sdt_getrecordrunningstatus
f1_keywords:
- dvbsiparser/IDVB_SDT.GetRecordRunningStatus
dev_langs:
- c++
req.header: dvbsiparser.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: 
req.target-min-winversvr: 
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: 
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- COM
api_location:
- dvbsiparser.h
api_name:
- IDVB_SDT.GetRecordRunningStatus
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IDVB_SDT::GetRecordRunningStatus


## -description



This topic applies to Update Rollup 2 for Microsoft Windows XP Media Center Edition 2005 and later.
        



The <b>GetRecordRunningStatus</b> method returns the running status of a particular service in the SDT.


## -parameters




### -param dwRecordIndex [in]

Specifies the record number for the service, indexed from zero. Call <a href="https://docs.microsoft.com/previous-versions/windows/desktop/api/dvbsiparser/nf-dvbsiparser-idvb_sdt-getcountofrecords">IDVB_SDT::GetCountOfRecords</a> to get the number of records in the SDT.


### -param pbVal [out]

Pointer to a variable that receives the running_status field. See the Remarks section in the <a href="https://docs.microsoft.com/previous-versions/windows/desktop/api/dvbsiparser/nf-dvbsiparser-idvb_rst-getrecordrunningstatus">IDVB_RST::GetRecordRunningStatus</a> method for more information.


## -returns



The method returns an <b>HRESULT</b>. Possible values include those in the following table.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_POINTER</b></dt>
</dl>
</td>
<td width="60%">
NULL pointer argument.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>MPEG2_E_OUT_OF_BOUNDS</b></dt>
</dl>
</td>
<td width="60%">
Index out of bounds.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">
The method succeeded.

</td>
</tr>
</table>
 




## -see-also




<a href="https://docs.microsoft.com/previous-versions/windows/desktop/api/dvbsiparser/nn-dvbsiparser-idvb_sdt">IDVB_SDT Interface</a>
 

 

