---
# required metadata

title: Master plans overview
description: Use various master plans to support your company's daily working operations, simulate different planning strategies that you want to monitor, and implement a company policy, such as a policy about internal performance or customer satisfaction. 
author: ChristianRytt
ms.date: 05/28/2020
ms.topic: article
ms.prod: 
ms.technology: 

# optional metadata

ms.search.form: ReqParameters, ReqPlanSched
# ROBOTS: 
audience: Application User
# ms.devlang: 
ms.reviewer: kamaybac
# ms.tgt_pltfrm: 
ms.custom: ["7911", "intro-internal"]
ms.assetid: a116b7de-3d6d-4321-87ba-5a5d99c2f64e
ms.search.region: Global
ms.search.industry: Manufacturing
ms.author: crytt
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0

---

# Master plans overview

[!include [banner](../includes/banner.md)]

Use various master plans to support your company's daily working operations, simulate different planning strategies that you want to monitor, and implement a company policy, such as a policy about internal performance or customer satisfaction.

You can configure master plans on the **Master plans** page.

There are two types of plans:

- **Static plan** – The master planning calculation uses the current data to generate a net requirements plan. This plan remains unchanged until the next time that you run master planning or manually change the plan. This is an operating plan that various company personnel, such as a purchaser or production planner, can use to base their decisions on and perform their daily activities.
- **Dynamic plan** – This plan starts with the same net requirements plan that was generated by master planning. However, you can update the dynamic plan every time that the master data changes. This could be when you create a new sales order, for example. This enables you to monitor the changing order network and item availability without disturbing the static plan that others are using for their work processes.

A company may choose to work with just a dynamic plan or it may use both static and dynamic plans. In addition, you can configure any master plan to reflect a particular strategy or address an issue. Examples are as follows:

- Set higher inventory levels to guarantee against stockouts.
- Set longer safety margins to protect against unreliable vendors.

You can also set up the starting dynamic plan so that it is updated with the new requirements plan every time that you run master planning. You can specify these settings on the **Master planning parameters** page.

## Additional resources

- [Coverage settings](coverage-settings.md)
- [Separating tactical and operative planning for master scheduling](https://community.dynamics.com/ax/b/dynamicsaxmanufacturingrdteamblog/posts/separating-tactical-and-operative-planning-for-master-scheduling)
- [Master Planning: Use a static and dynamic Master Plan or use one plan?](https://community.dynamics.com/ax/b/msdynaxlessonslearned/archive/2014/01/16/master-planning-use-a-static-and-dynamic-master-plan-or-use-one-plan)

[!INCLUDE[footer-include](../../includes/footer-banner.md)]
