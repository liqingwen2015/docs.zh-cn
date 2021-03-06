---
title: "填充字符串"
description: "填充字符串"
keywords: ".NET、.NET Core"
author: stevehoag
ms.author: shoag
ms.date: 07/26/2016
ms.topic: article
ms.prod: .net
ms.technology: dotnet-standard
ms.devlang: dotnet
ms.assetid: 1c8b3b44-d370-49e1-90b5-64ac81c02ae91c8b3b44-d370-49e1-90b5-64ac81c02ae9
translationtype: Human Translation
ms.sourcegitcommit: 90fe68f7f3c4b46502b5d3770b1a2d57c6af748a
ms.openlocfilehash: bc3cc9028b232cc2ba6ca3130c4bdb261c4a0a42
ms.lasthandoff: 03/02/2017

---

# <a name="padding-strings"></a>填充字符串

使用以下 [System.String](xref:System.String) 方法之一可创建由使用前导或尾随字符填充到指定总长度的原始字符串组成的新字符串。 填充字符可以是空格或指定字符，因而显示为右对齐或左对齐。

方法名称 | 使用
----------- | ---
[String.PadLeft](xref:System.String.PadLeft(System.Int32)) | 使用前导字符将字符串填充到指定总长度。
[String.PadRight](xref:System.String.PadRight(System.Int32)) | 使用尾随字符将字符串填充到指定总长度。

## <a name="padleft"></a>PadLeft

[String.PadLeft](xref:System.String.PadLeft(System.Int32)) 方法将足够前导填充字符连接到原始字符串来达到指定总长度，从而创建新字符串。 [String.PadLeft(Int32)](xref:System.String.PadLeft(System.Int32)) 方法使用空格作为填充字符，[String.PadLeft(Int32, Char)](xref:System.String.PadLeft(System.Int32,System.Char)) 方法使你可以指定自己的填充字符。

下面的代码示例使用 [PadLeft(Int32, Char)](xref:System.String.PadLeft(System.Int32,System.Char)) 方法创建一个长度为&20; 个字符的新字符串。 该示例向控制台显示“`--------Hello World!`”。

```csharp
string MyString = "Hello World!";
Console.WriteLine(MyString.PadLeft(20, '-'));
```

```vb
Dim MyString As String = "Hello World!"
Console.WriteLine(MyString.PadLeft(20, "-"c))
```

## <a name="padright"></a>PadRight

[String.PadRight](xref:System.String.PadRight(System.Int32)) 方法将足够尾随填充字符连接到原始字符串来达到指定总长度，从而创建新字符串。 [String.PadRight(Int32)](xref:System.String.PadRight(System.Int32)) 方法使用空格作为填充字符，[String.PadRight(Int32, Char)](xref:System.String.PadRight(System.Int32,System.Char)) 方法使你可以指定自己的填充字符。

下面的代码示例使用 [PadRight(Int32, Char)](xref:System.String.PadRight(System.Int32,System.Char)) 方法创建一个长度为&20; 个字符的新字符串。 该示例向控制台显示“`Hello World!--------`”。

```csharp
string MyString = "Hello World!";
Console.WriteLine(MyString.PadRight(20, '-'));
```

```vb
Dim MyString As String = "Hello World!"
Console.WriteLine(MyString.PadRight(20, "-"c))
```

## <a name="see-also"></a>另请参阅

[基本字符串操作](basic-string-operations.md)


