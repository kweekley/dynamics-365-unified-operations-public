---
title: Upload assets by using Azure Pipelines
description: This topic explains how you can upload assets to the Asset library in Microsoft Dynamics Lifecycle Services (LCS) by using Azure Pipelines.
author: jorisdg
ms.date: 03/05/2020
ms.topic: article
audience: Developer
ms.reviewer: tfehr
ms.custom: 26731
ms.search.region: Global
ms.author: jorisde
ms.search.validFrom: 2020-08-19
ms.dyn365.ops.version: AX 7.0.0
---

# Upload assets by using Azure Pipelines

You can automate the upload of assets to the Asset library in Microsoft Dynamics Lifecycle Services (LCS) by using the **Deploy Lifecycle Services (LCS) Asset Upload** task in Azure DevOps. This task is available only in **Releases** pipelines.

This topic assumes you have a working knowledge of [Azure Pipelines](/azure/devops/pipelines/get-started/pipelines-get-started).

> [!NOTE]
> Before you can add these steps to a pipeline, the [Dynamics 365 Finance and Operations Tools](https://marketplace.visualstudio.com/items?itemName=Dyn365FinOps.dynamics365-finops-tools) extension for Azure DevOps must be enabled and installed in the Azure DevOps account. For more information about how to install an extension for an organization, see [Install extensions](/azure/devops/marketplace/install-extension).

## Add the task to a pipeline

To add the task to the build of your YML or Classic pipeline, search the task list for **Dynamics Lifecycle Services (LCS) Asset Upload**.

The following table describes the options that are available for this task.

| Input name | Mandatory | Description |
|---|---|---|
| LCS Connection | Yes | Select or create a service connection to LCS. For more information, see [Create an LCS connection in Azure Pipelines](pipeline-lcs-connection.md). |
| LCS Project ID | Yes | Enter the ID of the project in LCS that contains both the asset to deploy and the target environment. You can find the project ID at the end of the URL of your project's dashboard. |
| Type of asset | Yes | Select the type of asset to upload. |
| File to upload | Yes | Enter the path of the file that you want to upload into the Asset library in LCS. |
| LCS Asset Name | No | Enter the name to show for the asset in the Asset library. If you don't enter a name here, the file name will be used. |
| LCS Description | No | Enter the description to show for the asset in the asset details. |
| Wait for Validation | No | For asset types that require validation, use this check box to instruct the task to wait until validation of the asset has either succeeded or failed. |


[!INCLUDE[footer-include](../../../includes/footer-banner.md)]