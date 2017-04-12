---
title: "ISymUnmanagedWriter::DefineGlobalVariable Method | Microsoft Docs"
ms.custom: ""
ms.date: "03/30/2017"
ms.prod: ".net-framework"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "dotnet-clr"
ms.tgt_pltfrm: ""
ms.topic: "reference"
apiname: 
  - "ISymUnmanagedWriter.DefineGlobalVariable"
apilocation: 
  - "diasymreader.dll"
apitype: "COM"
f1_keywords: 
  - "ISymUnmanagedWriter::DefineGlobalVariable"
dev_langs: 
  - "C++"
helpviewer_keywords: 
  - "ISymUnmanagedWriter::DefineGlobalVariable method [.NET Framework debugging]"
  - "DefineGlobalVariable method [.NET Framework debugging]"
ms.assetid: 843c904a-8176-4d8f-bd47-b4d4c29f4c5c
caps.latest.revision: 8
author: "mairaw"
ms.author: "mairaw"
manager: "wpickett"
---
# ISymUnmanagedWriter::DefineGlobalVariable Method
Defines a single global variable.  
  
## Syntax  
  
```  
HRESULT DefineGlobalVariable(  
    [in] const WCHAR  *name,  
    [in] ULONG32      attributes,  
    [in] ULONG32      cSig,  
    [in, size_is(cSig)] unsigned char signature[],  
    [in] ULONG32      addrKind,  
    [in] ULONG32      addr1,  
    [in] ULONG32      addr2,  
    [in] ULONG32      addr3);  
```  
  
#### Parameters  
 `name`  
 [in] A pointer to a `WCHAR` that defines the global variable name.  
  
 `attributes`  
 [in] The global variable attributes.  
  
 `cSig`  
 [in] A `ULONG32` that indicates the size, in characters, of the `signature` buffer.  
  
 `signature`  
 [in] The global variable signature.  
  
 `addrKind`  
 [in] The address type.  
  
 `addr1`  
 [in] The first address for the parameter specification.  
  
 `addr2`  
 [in] The second address for the parameter specification.  
  
 `addr3`  
 [in] The third address for the parameter specification.  
  
## Return Value  
 S_OK if the method succeeds; otherwise, E_FAIL or some other error code.  
  
## Requirements  
 **Header:** CorSym.idl, CorSym.h  
  
## See Also  
 [ISymUnmanagedWriter Interface](../../../../docs/framework/unmanaged-api/diagnostics/isymunmanagedwriter-interface.md)   
 [DefineLocalVariable Method](../../../../docs/framework/unmanaged-api/diagnostics/isymunmanagedwriter-definelocalvariable-method.md)   
 [DefineGlobalVariable2 Method](../../../../docs/framework/unmanaged-api/diagnostics/isymunmanagedwriter2-defineglobalvariable2-method.md)