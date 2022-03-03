---
title: 联机托管说明
permalink: index.html
layout: home
ms.openlocfilehash: c612655617c9fb1f1baef2b3a78d0cb87f0e3d18
ms.sourcegitcommit: 525e69932921e8ce30e81ee0f98ad4a87cda64ea
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2021
ms.locfileid: "137820356"
---
# <a name="content-directory"></a>内容目录

下面列出了每个实验室练习和演示的超链接。

## <a name="labs"></a>实验室

{% assign labs = site.pages | where_exp:"page", "page.url contains '/Instructions/Labs'" %}
| 模块 | 实验室 |
| --- | --- | 
{% 表示实验室 % 中的活动}| {{ activity.lab.module }} | [{{ activity.lab.title }}{% if activity.lab.type %} - {{ activity.lab.type }}{% endif %}]({{ site.github.url }}{{ activity.url }}) |
{% endfor %}

