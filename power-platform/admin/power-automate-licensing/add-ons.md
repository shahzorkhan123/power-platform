---
title: "Capacity based licensing for Power Automate"
description: "Add-ons for Power Automate licensing."
author: msftman
ms.topic: overview
ms.date: 05/01/2024
ms.author: kenseongtan
ms.reviewer: angieandrews
search.audienceType: 
  - admin
---

# Capacity based licensing for Power Automate

Add-ons can be added onto a standalone Power Automate license.

## Power Automate capacity add-ons

Power Apps and Power Automate capacity add-ons increase the daily Power Platform requests limits for workloads that need more usage capacity than their allocation. These add-ons provide an additional 50,000 daily Power Platform requests per unit for $50/month. Unused Power Platform requests don't carry over from day to day. You can purchase these add-ons at any time and they remain part of the subscription for the remainder of the subscription term.

You can't assign Power Platform requests capacity add-on packs to users or flows during the [transition period](types.md#transition-period). However, Microsoft recommends that you purchase these add-ons to remain within your license terms and to be prepared for when the transition period ends.

If Power Automate is throttling your flows, try [Pay-as-you-go](types.md#power-platform-requests-pay-as-you-go) to ensure that none of the flows in the environment are throttled. If you can't use Pay-as-you-go, purchase add-ons and create a Microsoft support ticket with the flow details and add-on details so that the support team can provide exceptions for your throttled flows.

## Hosted process (previously Power Automate hosted RPA add-on)

Desktop flows can have varying levels of workload throughout a period of time. For example, desktop flows for processing invoices or schedule reconciliation across multiple systems might have a monthly peak period. As desktop flows require a physical or virtual machine to run on, most organizations would provision machines to cope with requests during peak periods, leaving machine underutilized for most of the remaining time.

The Power Automate Hosted Process license provides Microsoft hosted machine capacity, enabling RPA with zero infrastructure. The Hosted Process license supports two scenarios:
- Individual hosted machines, enable developers to build or test automation and business users to run automation.
- Hosted machine groups, automatically scale workloads to optimize unattended automation in production, delivering improved business process continuity and governance at scale.

The following are important points you should be aware of regarding the Hosted Process license:
- One Hosted Process license includes the capacity to one Microsoft hosted machine and unattended RPA bot. All desktop flows (RPA) running on the machine and cloud flows (DPA) that are part of the business process are also covered by the license.
- One Hosted Process license can also be used as a process license to run unattended automation on a customer managed bot machine.
- You can purchase more AI Builder capacity; AI Builder service credit capacity is pooled at the tenant level.
- Any services or applications the unattended bot accesses must be licensed separately. For instance, if the bot is accessing Windows or Office, the Microsoft 365, you must purchase the unattended license in addition to the Power Automate Hosted Process license.
  
> [!NOTE]
> The Hosted Process licenses the machines and not the user. The Premium user plan is required to run attended RPA, and for RPA developers to build and manage desktop flows on the Power Automate portal. To learn more about the Premium RPA features that come with the Premium user plan, go to [Premium RPA features](/power-automate/desktop-flows/premium-features).

## Unattended RPA add-on

> [!NOTE]
> The Power Automate unattended RPA add-on is now replaced by the Power Automate Process plan.

Unattended desktop flows run without human interaction. These flows are best for scenarios such as processing invoices and entering them into a legacy application automatically or scheduled financial reconciliation across multiple systems that can only be automated by clicking user interfaces.

When running unattended, Power Automate securely signs into the device on your behalf, executes the desktop flow actions on the target applications, and then signs out of the device.

The Power Automate unattended RPA add-on extends desktop-based automation by enabling a bot to run autonomously (independent of a user). Unattended bots can be deployed on a local or remote desktop, or in a virtualized environment. The Power Automate per user with attended RPA or Power Automate per flow plans are the eligible standalone offers for the unattended RPA add-on.

> [!NOTE]
> The Power Automate unattended RPA add-on is licensed by a bot. Concurrent instances of a singular process require an additional unattended bot for each instance. Multiple unattended RPA add-ons can be applied against a qualifying base license (user license or flow license).

Here are a few important notes of which you should be aware regarding the unattended add-on.

- One unattended RPA add-on license includes the rights to one unattended RPA bot.
- If you run the unattended RPA bot in a virtual machine, you must purchase the necessary compute resources.
- You can purchase additional AI Builder capacity; AI Builder service credit capacity is pooled at the tenant level.
- Any services or applications the unattended bot accesses must be licensed separately. For instance, if the bot is accessing Windows or Microsoft 365, you must purchase the unattended license in addition to the Power Automate unattended RPA add-on.

### FAQs about the unattended add-on

1. I want to run unattended flow. What licenses do I need?

   You need either **Power Automate Premium plan** (previously Power Automate per user plan with attended RPA) or Power Automate per flow plans as a base license and Unattended add-on to be able to run the unattended flow.

1. I need multiple instances running unattended. Do I need multiple add-ons?

   Yes, if you need to run them at the same time. If not, the runs are queued and begin when the bot is free.

## AI builder capacity add-on

AI Builder is licensed as an add-on to standalone Power Apps and Power Automate licensing and to Dynamics 365 licenses. AI Builder is licensed on a capacity basis. AI Builder capacity is expressed as *service credits*. Service credits serve as the single (common) currency across all the scenarios supported by AI Builder. The available service credits decrease when you use AI Builder services. Different scenarios (for example, forms processing, prediction, etc.) use service credits at different rates. Purchase the appropriate number of AI Builder capacity add-on units based on anticipated usage across all scenarios.

Each unit of AI Builder capacity add-on includes 1 million service credits per month. For example, a customer who requires 4.7 million service credits per month (based on anticipated usage), should purchase five units of AI Builder capacity add-on.

> [!NOTE]
>
> - Purchased service credits can be used from AI Builder models included within Power Automate, Power Apps, and Dynamics 365 applications.
> - Service credits are deducted / consumed for both training and production usage
> - Service credits are pooled across the tenant.

### FAQs about the AI builder add-on

I have a Power Automate per user with RPA plan and I got AI builder credits as part of the plan. Can I transfer the credits to someone else?

No. AI builder service credits are pooled at the tenant level and can't be assigned to a particular user. So, any user who runs a flow that needs AI builder service credits needs to use credits from the pool.

[!INCLUDE[footer-include](../../includes/footer-banner.md)]
