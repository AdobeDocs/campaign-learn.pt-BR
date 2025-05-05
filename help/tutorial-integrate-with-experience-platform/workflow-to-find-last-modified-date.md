---
title: Criar um fluxo de trabalho de exportação (Parte 1) - Encontre a data da última modificação para uma lista de destinatários
description: Nesta primeira parte do tutorial Criar um fluxo de trabalho de exportação, saiba como criar um fluxo de trabalho que encontra a data da última modificação de uma lista de destinatários criados de um segmento da Experience Platform.
feature: Data Management, Workflows
jira: KT-8162
thumbnail: 336387.jpg
doc-type: feature video
activity: setup
team: TM
role: Admin
level: Beginner, Experienced
exl-id: 6fd70eea-3be7-4589-a608-05b0a8de93a6
source-git-commit: 116a24a8aa123f615e08fa4ebd187b3c4c460ba2
workflow-type: tm+mt
source-wordcount: '125'
ht-degree: 100%

---

# Criar um fluxo de trabalho de exportação (Parte 1) - Encontre a data da última modificação para uma lista de destinatários

Nesta primeira parte do tutorial Criar um fluxo de trabalho de exportação, saiba como criar um fluxo de trabalho que encontra a data da última modificação de uma lista de destinatários criados de um segmento da Experience Platform.

>[!VIDEO](https://video.tv.adobe.com/v/3450052?quality=12&learn=on&captions=por_br){transcript=true}

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
