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
TQID: 'https://experienceleague.adobe.com/0C-fRmXsfzB-1kePFSNtzUFtqPHDQ1wW1LH2-6Zuw5g'
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
  - id: d0e9f0b2-1f2b-4134-9844-49cd4e950f27
    internal-label: Campaign v8
feature_v2:
  - id: a658c786-869b-4194-a780-2594d663adda
    internal-label: Data management
subfeature_v2:
  - id: fcb46c0f-76e1-48bc-9dd0-fcf9d97526cf
    internal-label: Workflows
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
    internal-label: Beginner
  - id: d378ca77-2da1-4f39-ad92-1917fe974a38
    internal-label: Experienced
topic_v2:
  - id: ebde5b41-29c9-4f5e-9ef6-1197e85409e3
    internal-label: Data management
source-git-commit: 369f9c3691b6326e521ebc9139aac1d2ee7c3ce2
workflow-type: tm+mt
source-wordcount: '123'
ht-degree: 100%
---
# Criar um fluxo de trabalho de exportação (Parte 1) - Encontre a data da última modificação para uma lista de destinatários

Nesta primeira parte do tutorial Criar um fluxo de trabalho de exportação, saiba como criar um fluxo de trabalho que encontra a data da última modificação de uma lista de destinatários criados de um segmento da Experience Platform.

>[!VIDEO](https://video.tv.adobe.com/v/336387?quality=12&learn=on){transcript=true}

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
