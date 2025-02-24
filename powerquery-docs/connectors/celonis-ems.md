---
title: Power Query Celonis EMS connector
description: Provides basic information, prerequisites, and connection steps for Celonis EMS.
author: capono
ms.date: 7/13/2023 
ms.author: bezhan
---

# Celonis EMS (Beta)

## Summary

| Item | Description |
| ---- | ----------- |
| Release State | Beta |
| Products | Power BI (Datasets) </br> Power BI (Dataflows)<br/>Fabric (Dataflow Gen2) |
| Authentication Types Supported | Organizational Account |
| Function Reference Documentation | [Web.Contents](/powerquery-m/web-contents) </br> [Parquet.Document](/power-query/connectors/parquet) </br> [Json.Document](/powerquery-m/json-document) </br> [Json.FromValue](/powerquery-m/json-fromvalue)|

## Prerequisites

Before you can sign in to [Celonis EMS](https://celon.is/EMS-Platform), you must have a Celonis EMS account (username/password).

## Capabilities Supported

* Import
* Navigate using full hierarchy

## Connect to Celonis EMS from Power Query Desktop

To make the connection, take the following steps:

1. Select **Get Data** from the **Home** ribbon in Power BI Desktop. Select **Celonis EMS** in the connector selection and then select **Connect**.

![Screenshot of Get Data dialog showing the Celonis EMS connector selected.](media/celonis-ems/get-data.png)

1. The **Celonis EMS** dialog now appears, with an example URL. Enter your Celonis EMS Team URL and then select **OK**.

![Screenshot of the Celonis EMS dialog with the Celonis EMS URL entered.](media/celonis-ems/set-url.png)

1. Enter your **Application Key** or your **Personal API Key** generated in the Celonis EMS.

![Screenshot of the authentication dialog where you enter your key for authentication.](media/celonis-ems/authentication.png)
  
1. Once you're done, select **Connect**.
  
1. Upon a successful connection, the **Navigator** opens with the list of packages available in the given EMS team. Select the **Knowledge Model Record** you want to import and then select **Load**.

![Navigate to package](media/celonis-ems/navigator.png)

## Limitations and issues

You should be aware of the following limitations and issues associated with accessing Celonis EMS data:

* Celonis EMS has a built-in limit of 200 K rows and 20 columns returned per record.

* Only defined records can be imported. Auto-generated records are excluded here.
