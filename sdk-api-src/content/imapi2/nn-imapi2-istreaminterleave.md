---
UID: NN:imapi2.IStreamInterleave
title: IStreamInterleave (imapi2.h)
description: Use this interface to combine several data streams into a single stream by alternately interspersing portions of each.helpviewer_keywords: ["IStreamInterleave","IStreamInterleave interface [IMAPI]","IStreamInterleave interface [IMAPI]","described","imapi.istreaminterleave","imapi2/IStreamInterleave"]
old-location: imapi\istreaminterleave.htm
tech.root: imapi
ms.assetid: 2d0f03e5-a47d-4b46-a177-f462bbafe153
ms.date: 12/05/2018
ms.keywords: IStreamInterleave, IStreamInterleave interface [IMAPI], IStreamInterleave interface [IMAPI],described, imapi.istreaminterleave, imapi2/IStreamInterleave
f1_keywords:
- imapi2/IStreamInterleave
dev_langs:
- c++
req.header: imapi2.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista, Windows XP with SP2 [desktop apps only]
req.target-min-winversvr: Windows Server 2003 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Imapi2.idl
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
- imapi2.h
api_name:
- IStreamInterleave
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IStreamInterleave interface


## -description


Use this interface to combine several data streams into a single stream by alternately interspersing portions of each. You create interleaved streams when data streams need to run parallel to each other instead of sequentially. For example, some CD formats require user data interleaved with the subcode information. Any fixed-size interleave is supported.

To create an instance of this interface, call the <b>CoCreateInstance</b> function. Use__uuidof(MsftStreamInterleave) for the class identifier and __uuidof(IStreamInterleave) for the interface identifier.


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IStreamInterleave</b> interface inherits from <b>IStream</b>. <b>IStreamInterleave</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IStreamInterleave</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://docs.microsoft.com/windows/desktop/api/imapi2/nf-imapi2-istreaminterleave-initialize">Initialize</a>
</td>
<td align="left" width="63%">
Initializes this interleaved stream from an array of input streams and interleave sizes.

</td>
</tr>
</table> 


## -remarks



To create the <b>MsftStreamInterleave</b> object in a script, use IMAPI2.MsftStreamInterleave as the program identifier when calling <b>CreateObject</b>.




## -see-also




<a href="https://docs.microsoft.com/windows/desktop/api/imapi2/nn-imapi2-istreamconcatenate">IStreamConcatenate</a>



<a href="https://docs.microsoft.com/windows/desktop/api/imapi2/nn-imapi2-istreampseudorandombased">IStreamPseudoRandomBased</a>
 

 

