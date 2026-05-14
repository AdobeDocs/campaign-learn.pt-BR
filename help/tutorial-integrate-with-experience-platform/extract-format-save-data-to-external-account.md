---
title: Criar um fluxo de trabalho de exportação (Parte 2) - Extrair, formatar e salvar dados em uma conta externa
description: Nesta segunda parte do tutorial Criar um fluxo de trabalho de exportação, você aprenderá a formatar os dados para exportação e a salvar os dados em uma conta externa.
feature: Data Management, Workflows
jira: KT-8160
thumbnail: 336391.jpg
doc-type: feature video
activity: setup
team: TM
role: Admin
level: Beginner, Experienced
exl-id: ac29b75c-a838-4183-8ec5-034281290725
TQID: https://experienceleague.adobe.com/WLEORmaWuZubXGHSTB5qC7dm8ZiMau6weKy48fq0q-0
product_v2: id: dfc56824-e8b9-499e-85d4-21aedb507314
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
level_v2: id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
topic_v2: id: ebde5b41-29c9-4f5e-9ef6-1197e85409e3
source-git-commit: 1f6ccc9f0e59ce16a4e781d2d366cf0257b1c8aa
workflow-type: tm+mt
source-wordcount: 94
ht-degree: 100%

---

# Criar um fluxo de trabalho de exportação (Parte 2): extrair, formatar e salvar dados em uma conta externa

Nesta segunda parte do tutorial Criar um fluxo de trabalho de exportação, você aprenderá a formatar os dados para exportação e a salvar os dados em uma conta externa.

>[!VIDEO](https://video.tv.adobe.com/v/336391?quality=12&learn=on){transcript=true}

## Assets

JavaScript: salvar data

```java
 logInfo("=====================")
 logInfo("Starting Execution...")

 optionName = vars.OPTION_NAME;
 logInfo("optionName: " + optionName);
 logInfo("NEXT Run Date: " + vars.nextRunTime);
 
 //Make sure we have valid values before saving for next run
 if (vars.nextRunTime == null || optionName == null){

   logInfo("Unable to find non-null values for optionName/nextRunTime! Throwing Error.")
   throw new Error('Unable to find non-null values for optionName/nextRunTime!  Ending Execution.');

 } else {

   // Save the nextRunTime to the database to establish starting point for next run.
   setOption(optionName, vars.nextRunTime);
   logInfo("Date Saved. [" + optionName + "] = [" + vars.lastRunTime + "]")

 }

 logInfo("Finished Execution.") 
 logInfo("===================")
```
