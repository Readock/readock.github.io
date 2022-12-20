---
layout: page
title: Style Visualization
description: See the various html elements all on one page
categories: [test]
tags: [test]     # TAG names should always be lowercase
author: felix
---

# Header 1 `code` [link](./) and [`code` link](./)
## Header 2 `code` [link](./) and [`code` link](./)
### Header 3 `code` [link](./) and [`code` link](./)
#### Header 4 `code` [link](./) and [`code` link](./)
##### Header 5 `code` [link](./) and [`code` link](./)
###### Header 6 `code` [link](./) and [`code` link](./)

Paragraph with `code` and [link](./) and [`code` link](./)

| Plain | Code   | Link       | Ymark                            | Nmark                           | Arrows       |
|-------|--------|------------|----------------------------------|---------------------------------|--------------|
| text  | `text` | [text](./) | ![yes](/assets/icons/Ymark.png) | ![no](/assets/icons/Nmark.png) | 🡐 🡒 🡑 🡓 « » |

- Bullet list
- with `code`
- and [link](./)

1. Ordered list
3. with `code`
4. and [link](./)

paragraph with a <tip>&lt;tip/&gt;</tip> in it

paragraph with a <todo>&lt;todo/&gt;</todo> in it

paragraph with a <problem>&lt;problem/&gt;</problem> in it


------------------------------------------------------------

<todo-p>
Value inside &lt;todo-p/&gt; tag
</todo-p>

------------------------------------------------------------

paragraph between h rules

------------------------------------------------------------

multiple h rules in a row

------------------------------------------------------------
------------------------------------------------------------
------------------------------------------------------------

### C++ Code

```c++
UCLASS(DisplayName="Unreal Name")
class UFoo : public UObject
{
    // Test if Github's C++ processor has UE preprocessor support
    UPROPERTY(BlueprintReadWrite, Category="Xist")
    bool bHopeForSuccess = true;
    Foo(const FObjectInitializer& ObjectInitializer = FObjectInitializer::Get())
      : Super(ObjectInitializer)
      {}
};
```

![assets](/assets/bms.png){:width="50%"}

{% youtube f_Pcu6wTzoA %}