---
UID: NF:winldap.ldap_control_freeW
title: ldap_control_freeW function (winldap.h)
description: The ldap_control_free function frees an LDAPControl structure.helpviewer_keywords: ["_ldap_ldap_control_free","ldap.ldap__control__free","ldap.ldap_control_free","ldap_control_free","ldap_control_free function [LDAP]","ldap_control_freeA","ldap_control_freeW","winldap/ldap_control_free","winldap/ldap_control_freeA","winldap/ldap_control_freeW"]
old-location: ldap\ldap_control_free.htm
tech.root: ldap
ms.assetid: 10729355-8f80-477b-acc8-705db72cebdb
ms.date: 12/05/2018
ms.keywords: _ldap_ldap_control_free, ldap.ldap__control__free, ldap.ldap_control_free, ldap_control_free, ldap_control_free function [LDAP], ldap_control_freeA, ldap_control_freeW, winldap/ldap_control_free, winldap/ldap_control_freeA, winldap/ldap_control_freeW
f1_keywords:
- winldap/ldap_control_free
dev_langs:
- c++
req.header: winldap.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista
req.target-min-winversvr: Windows Server 2008
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: ldap_control_freeW (Unicode) and ldap_control_freeA (ANSI)
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Wldap32.lib
req.dll: Wldap32.dll
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- DllExport
api_location:
- Wldap32.dll
api_name:
- ldap_control_free
- ldap_control_freeA
- ldap_control_freeW
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# ldap_control_freeW function


## -description


The <b>ldap_control_free</b> function frees an 
   <a href="https://docs.microsoft.com/previous-versions/windows/desktop/api/winldap/ns-winldap-ldapcontrola">LDAPControl</a> structure.


## -parameters




#### - Control [in]

The <a href="https://docs.microsoft.com/previous-versions/windows/desktop/api/winldap/ns-winldap-ldapcontrola">LDAPControl</a> structure to free.


## -returns



If the function succeeds, <b>LDAP_SUCCESS</b> is returned.

If the function fails, an error code is returned. For more information, see 
       <a href="https://docs.microsoft.com/previous-versions/windows/desktop/ldap/return-values">Return Values</a>.




## -remarks



Use this function to free an <a href="https://docs.microsoft.com/previous-versions/windows/desktop/api/winldap/ns-winldap-ldapcontrola">LDAPControl</a> structure 
     previously allocated by an LDAP function call, such as one allocated by a call to 
     <a href="https://docs.microsoft.com/previous-versions/windows/desktop/api/winldap/nf-winldap-ldap_create_page_control">ldap_create_page_control</a> or 
     <a href="https://docs.microsoft.com/previous-versions/windows/desktop/api/winldap/nf-winldap-ldap_create_vlv_controla">ldap_create_vlv_control</a>.

<div class="alert"><b>Note</b>  This function should only be used to free a control created internally by LDAP API functions. It is not used 
     to free memory that is explicitly allocated by the user program.</div>
<div> </div>



## -see-also




<a href="https://docs.microsoft.com/previous-versions/windows/desktop/ldap/functions">Functions</a>



<a href="https://docs.microsoft.com/previous-versions/windows/desktop/api/winldap/ns-winldap-ldapcontrola">LDAPControl</a>



<a href="https://docs.microsoft.com/previous-versions/windows/desktop/ldap/return-values">Return Values</a>



<a href="https://docs.microsoft.com/previous-versions/windows/desktop/api/winldap/nf-winldap-ldap_create_page_control">ldap_create_page_control</a>



<a href="https://docs.microsoft.com/previous-versions/windows/desktop/api/winldap/nf-winldap-ldap_create_vlv_controla">ldap_create_vlv_control</a>
 

 

