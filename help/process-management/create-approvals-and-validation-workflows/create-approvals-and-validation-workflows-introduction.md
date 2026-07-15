---
title: Criar fluxos de trabalho de aprovação e validação - Introdução
description: Saiba como configurar diferentes fluxos de trabalho de validação e aprovação.
feature: Workflows, Approvals
doc-type: feature video
activity: setup
team: TM
role: User
level: Intermediate
recommendations: noDisplay
exl-id: fa4c2180-15bb-424b-a54e-c7d744385fb6
TQID: https://experienceleague.adobe.com/nVZT-SWtytNyXrkbV-J7LWhR5-KHo601s0dE9yUiOaY
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
feature_v2:
  - id: a075b2c1-7748-4328-b7f6-343aa314616a
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
source-git-commit: 1f6ccc9f0e59ce16a4e781d2d366cf0257b1c8aa
workflow-type: ht
source-wordcount: 267
ht-degree: 100%

---

# Criar fluxos de trabalho de aprovação e validação - Introdução

O Adobe Campaign oferece várias opções para que profissionais de marketing possam revisar e fornecer conteúdo de entregas, direcionamento de campanha, extração de dados e aprovações de orçamento. Saiba como [gerenciar aprovações](/help/process-management/create-approvals-and-validation-workflows/manage-approvals.md).

## Pré-requisito {#prerequisite}

Antes de habilitar as etapas de aprovação, a equipe de marketing deve definir revisores individuais:

* A função de revisor do Adobe Campaign em uma atividade de aprovação pode ser um único revisor (Operador) ou um grupo de revisores (função Operador).
* Para permitir que os desenvolvedores de campanha selecionem os revisores como aprovadores em uma campanha ou entrega, os revisores e os grupos de revisores devem ser configurados no Adobe Campaign por um administrador.

## Configuração de aprovações {#configuring-approvals}

1. [Configurar aprovações para campanhas](/help/process-management/create-approvals-and-validation-workflows/configure-approvals-for-campaigns.md):
Se você tiver o mesmo conjunto de revisores para todas as entregas no fluxo de trabalho da campanha, aplique a funcionalidade de aprovação da campanha configurando aprovações e revisores no nível da campanha. As tarefas de aprovação e os revisores são encaminhados para cada atividade de entrega do fluxo de trabalho depois que ele for executado.
2. [Configurar aprovações para entregas](/help/process-management/create-approvals-and-validation-workflows/configure-approvals-for-deliveries.md):
Você também pode configurar aprovações em um nível de entrega. Se as etapas de aprovação de entrega e os revisores forem diferentes das etapas de aprovação da campanha e seus revisores, as configurações de entrega substituirão as configurações da campanha.
3. [Criar um processo de aprovação em um fluxo de trabalho](/help/process-management/create-approvals-and-validation-workflows/create-approval-process-in-a-workflow.md):
A atividade de aprovação permite a criação de um processo de aprovação dentro de um fluxo de trabalho. Dessa forma, a lógica de seleção de direcionamento pode ser aprovada antes que a entrega seja iniciada. Ela também permite a aprovação em vários níveis no fluxo de trabalho, se necessário.

Para obter mais informações, consulte a [documentação](https://experienceleague.adobe.com/docs/campaign-classic/using/automating-with-workflows/flow-control-activities/approval.html?lang=pt-BR).
