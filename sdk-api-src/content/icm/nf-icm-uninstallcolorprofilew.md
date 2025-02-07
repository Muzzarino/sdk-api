---
UID: NF:icm.UninstallColorProfileW
title: UninstallColorProfileW
description: Removes a specified color profile from a specified computer. Associated files are optionally deleted from the system.
tech.root: wcs
ms.date: 02/01/2021
targetos: Windows
req.assembly: 
req.construct-type: function
req.ddi-compliance: 
req.dll: Mscms.dll
req.header: icm.h
req.idl: 
req.include-header: 
req.irql: 
req.kmdf-ver: 
req.lib: Mscms.lib
req.max-support: 
req.namespace: 
req.redist: 
req.target-min-winverclnt: Windows 2000 Professional \[desktop apps only\]
req.target-min-winversvr: Windows 2000 Server \[desktop apps only\]
req.target-type: 
req.type-library: 
req.umdf-ver: 
req.unicode-ansi: 
topic_type:
 - apiref
api_type:
 - 
api_location:
 - mscms.dll
api_name:
 - UninstallColorProfileW
 - UninstallColorProfile
f1_keywords:
 - UninstallColorProfileW
 - icm/UninstallColorProfileW
 - UninstallColorProfile
 - icm/UninstallColorProfile
dev_langs:
 - c++
---

## -description

Removes a specified color profile from a specified computer. Associated files are optionally deleted from the system.

## -parameters

### -param pMachineName

Reserved. Must be **NULL**. This parameter is intended to point to the name of the machine from which to uninstall the specified profile. A **NULL** pointer indicates the local machine.

### -param pProfileName

Points to the file name of the profile to uninstall.

### -param bDelete

If set to **TRUE**, the function deletes the profile from the COLOR directory. If set to **FALSE**, this function has no effect.

## -returns

If this function succeeds, the return value is **TRUE**.

If this function fails, the return value is **FALSE**. For extended error information, call **GetLastError**.

## -remarks

## -see-also

* [Basic color management concepts](ms536813\(v=vs.85\).md)
* [Functions](/windows/win32/wcs/functions)
