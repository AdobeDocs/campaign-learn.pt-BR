---
title: Criar um fluxo de trabalho de exportação (Parte 1) - Encontre a data da última modificação para uma lista de recipients
description: Nesta primeira parte do tutorial Criar um fluxo de trabalho de exportação, saiba como criar um fluxo de trabalho que encontra a data da última modificação de uma lista de recipients criados de um segmento da Experience Platform.
feature: Data Import/Export, Workflows
kt: 8162
thumbnail: 336387.jpg
doc-type: feature video
activity: setup
team: TM
role: Admin
level: Beginner, Experienced
exl-id: 6fd70eea-3be7-4589-a608-05b0a8de93a6
source-git-commit: b1b8d8a99a551239c445fb588cbd126b66a53c9b
workflow-type: ht
source-wordcount: '120'
ht-degree: 100%

---

# Criar um fluxo de trabalho de exportação (Parte 1) - Encontre a data da última modificação para uma lista de recipients

Nesta primeira parte do tutorial Criar um fluxo de trabalho de exportação, saiba como criar um fluxo de trabalho que encontra a data da última modificação de uma lista de recipients criados de um segmento da Experience Platform.

>[!VIDEO](https://video.tv.adobe.com/v/336387?quality=12&learn=on)

## Assets

JavaScript para estabelecer intervalos de datas:

```java
 var DEFAULT_LOOKBACK_DAYS = 90;
 vars.OPTION_NAME = "BroadLog_CaptureTime";

 logInfo("=====================");
 logInfo("Starting Execution...");

 // Establish the last and next RunTimes
 var lastRunTime = getOption(vars.OPTION_NAME);
 var nextRunTime = getCurrentDate();

 //To reset and run through DEFAULT_LOOKBACK, uncomment the following line.
 //lastRunTime = null;

 logInfo("NEXT Run Date Set: [" + nextRunTime + "]");
 logInfo("LAST Run Date Retrieved (" + lastRunTime + ")");

 //Check for null so we can default the lastRunTime using the DEFAULT_LOOKBACK 
 if (lastRunTime == null || lastRunTime == "null" || lastRunTime == "") {

   logInfo("Empty Date Retrieved, setting to default lookback (-" + DEFAULT_LOOKBACK_DAYS + " days)");
   lastRunTime = new Date();
   lastRunTime.setDate(nextRunTime.getDate() - DEFAULT_LOOKBACK_DAYS);
   logInfo("LAST Run Date Set: [" + lastRunTime + "]");

 } 

 //Persist values through execution of this instance of the workflow.
 vars.lastRunTime = lastRunTime;
 vars.nextRunTime = nextRunTime;

 logInfo("Finished Execution.");
 logInfo("===================");
```

## Próximo vídeo

[Criar um fluxo de trabalho de exportação (Parte 2) - Extrair, formatar e salvar dados em uma conta externa](extract-format-save-data-to-external-account.md)
