---
title: Criar um workflow de exportação (Parte 2) - Extrair, formatar e salvar dados em uma conta externa
description: Nesta segunda parte do tutorial Criar um fluxo de trabalho de exportação , você aprenderá a formatar os dados para exportação e a salvar os dados em uma conta externa. 
feature: Data Import/Export, Workflows
kt: 8160
thumbnail: 336391.jpg
doc-type: feature video
activity: setup
team: TM
role: Admin
level: Beginner, Experienced
source-git-commit: 75131bcf23154c05621bb6b63224ad906ec96ecd
workflow-type: tm+mt
source-wordcount: '92'
ht-degree: 0%

---


# Criar um workflow de exportação (Parte 2): Extrair, formatar e salvar dados em uma conta externa

Nesta segunda parte do tutorial Criar um fluxo de trabalho de exportação , você aprenderá a formatar os dados para exportação e a salvar os dados em uma conta externa.

>[!VIDEO](https://video.tv.adobe.com/v/336391?quality=12)

## Ativos

JavaScript: Salvar data

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
