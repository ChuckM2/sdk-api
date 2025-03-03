---
UID: NF:winreg.RegUnLoadKeyW
title: RegUnLoadKeyW function (winreg.h)
description: Unloads the specified registry key and its subkeys from the registry.helpviewer_keywords: ["RegUnLoadKey","RegUnLoadKey function","RegUnLoadKeyA","RegUnLoadKeyW","_win32_regunloadkey","base.regunloadkey","winreg/RegUnLoadKey","winreg/RegUnLoadKeyA","winreg/RegUnLoadKeyW"]
old-location: base\regunloadkey.htm
tech.root: SysInfo
ms.assetid: 73b4b6a9-4acb-4247-bd7f-82024ba3e14a
ms.date: 12/05/2018
ms.keywords: RegUnLoadKey, RegUnLoadKey function, RegUnLoadKeyA, RegUnLoadKeyW, _win32_regunloadkey, base.regunloadkey, winreg/RegUnLoadKey, winreg/RegUnLoadKeyA, winreg/RegUnLoadKeyW
f1_keywords:
- winreg/RegUnLoadKey
dev_langs:
- c++
req.header: winreg.h
req.include-header: Windows.h
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: RegUnLoadKeyW (Unicode) and RegUnLoadKeyA (ANSI)
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Advapi32.lib
req.dll: Advapi32.dll
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- DllExport
api_location:
- Advapi32.dll
- API-MS-Win-Core-Localregistry-l1-1-0.dll
- KernelBase.dll
- API-MS-Win-Core-Registry-l1-1-0.dll
- API-MS-Win-DownLevel-AdvApi32-l1-1-0.dll
- API-MS-Win-DownLevel-AdvApi32-l1-1-1.dll
- MinKernelBase.dll
- api-ms-win-core-registry-l1-1-1.dll
api_name:
- RegUnLoadKey
- RegUnLoadKeyA
- RegUnLoadKeyW
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# RegUnLoadKeyW function


## -description


Unloads the specified registry key and its subkeys from the registry.

 Applications that back up or restore system state including system files and registry hives should use the <a href="https://msdn.microsoft.com/library/aa384649(VS.85).aspx">Volume Shadow Copy Service</a> instead of the registry functions.


## -parameters




### -param hKey [in]

A handle to the registry key to be unloaded. This parameter can be a handle returned by a call to 
<a href="https://docs.microsoft.com/windows/desktop/api/winreg/nf-winreg-regconnectregistrya">RegConnectRegistry</a> function or one of the following predefined handles: 




<b>HKEY_LOCAL_MACHINE</b>
<b>HKEY_USERS</b>

### -param lpSubKey [in, optional]

The name of the subkey to be unloaded. The key referred to by the <i>lpSubKey</i> parameter must have been created by using the 
<a href="https://docs.microsoft.com/windows/desktop/api/winreg/nf-winreg-regloadkeya">RegLoadKey</a> function. 




Key names are not case sensitive.

For more information, see 
<a href="https://docs.microsoft.com/windows/desktop/SysInfo/registry-element-size-limits">Registry Element Size Limits</a>.


## -returns



If the function succeeds, the return value is ERROR_SUCCESS.

If the function fails, the return value is a nonzero error code defined in Winerror.h. You can use the 
<a href="https://docs.microsoft.com/windows/desktop/api/winbase/nf-winbase-formatmessage">FormatMessage</a> function with the FORMAT_MESSAGE_FROM_SYSTEM flag to get a generic description of the error.




## -remarks



This function removes a hive from the registry but does not modify the file containing the registry information. A hive is a discrete body of keys, subkeys, and values that is rooted at the top of the registry hierarchy.

The calling process must have the SE_RESTORE_NAME and SE_BACKUP_NAME privileges on the computer in which the registry resides. For more information, see 
<a href="https://docs.microsoft.com/windows/desktop/SecBP/running-with-special-privileges">Running with Special Privileges</a>.




## -see-also




<a href="https://docs.microsoft.com/windows/desktop/api/winreg/nf-winreg-regconnectregistrya">RegConnectRegistry</a>



<a href="https://docs.microsoft.com/windows/desktop/api/winreg/nf-winreg-regdeletekeya">RegDeleteKey</a>



<a href="https://docs.microsoft.com/windows/desktop/api/winreg/nf-winreg-regloadkeya">RegLoadKey</a>



<a href="https://docs.microsoft.com/windows/desktop/api/winreg/nf-winreg-regrestorekeya">RegRestoreKey</a>



<a href="https://docs.microsoft.com/windows/desktop/SysInfo/registry-functions">Registry Functions</a>



<a href="https://docs.microsoft.com/windows/desktop/SysInfo/registry">Registry Overview</a>
 

 

