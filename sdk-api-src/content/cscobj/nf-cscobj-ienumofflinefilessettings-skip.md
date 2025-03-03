---
UID: NF:cscobj.IEnumOfflineFilesSettings.Skip
title: IEnumOfflineFilesSettings::Skip (cscobj.h)
description: Skips over the next specified number of elements in the enumeration.helpviewer_keywords: ["IEnumOfflineFilesSettings interface [Offline Files]","Skip method","IEnumOfflineFilesSettings.Skip","IEnumOfflineFilesSettings::Skip","Skip","Skip method [Offline Files]","Skip method [Offline Files]","IEnumOfflineFilesSettings interface","cscobj/IEnumOfflineFilesSettings::Skip","of.ienumofflinefilessettings_skip"]
old-location: of\ienumofflinefilessettings_skip.htm
tech.root: offlinefiles
ms.assetid: 8b84fcef-f4e3-4e23-b254-dd21f145c1ba
ms.date: 12/05/2018
ms.keywords: IEnumOfflineFilesSettings interface [Offline Files],Skip method, IEnumOfflineFilesSettings.Skip, IEnumOfflineFilesSettings::Skip, Skip, Skip method [Offline Files], Skip method [Offline Files],IEnumOfflineFilesSettings interface, cscobj/IEnumOfflineFilesSettings::Skip, of.ienumofflinefilessettings_skip
f1_keywords:
- cscobj/IEnumOfflineFilesSettings.Skip
dev_langs:
- c++
req.header: cscobj.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista
req.target-min-winversvr: Windows Server 2008
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
req.dll: CscSvc.dll; CscObj.dll
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- COM
api_location:
- CscSvc.dll
- CscObj.dll
api_name:
- IEnumOfflineFilesSettings.Skip
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IEnumOfflineFilesSettings::Skip


## -description


Skips over the next specified number of elements in the enumeration.


## -parameters




### -param celt [in]

Number of elements to be skipped.


## -returns



Returns <b>S_OK</b> if the number of elements skipped is <i>celt</i>; S_FALSE if a number less than <i>celt</i> is skipped; or an error value otherwise.




## -see-also




<a href="https://docs.microsoft.com/previous-versions/windows/desktop/api/cscobj/nn-cscobj-ienumofflinefilessettings">IEnumOfflineFilesSettings</a>
 

 

