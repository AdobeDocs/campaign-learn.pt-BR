---
title: Criar workflows de aprovação e validação - Introdução
description: Saiba como configurar diferentes workflows de validação e aprovação.
feature: Workflows, Approvals
doc-type: feature video
activity: setup
team: TM
role: User
level: Intermediate
recommendations: noDisplay
exl-id: fa4c2180-15bb-424b-a54e-c7d744385fb6
source-git-commit: 4d21755204c22fbeb4ac3a2916e9ee68cd2e0f9a
workflow-type: ht
source-wordcount: '255'
ht-degree: 100%

---

# Criar workflows de aprovação e validação - Introdução

O Adobe Campaign oferece várias opções para que profissionais de marketing possam revisar e fornecer conteúdo de entregas, direcionamento de campanha, extração de dados e aprovações de orçamento. Saiba como [gerenciar aprovações](/help/process-management/create-approvals-and-validation-workflows/manage-approvals.md).

## Pré-requisito {#prerequisite}

Antes de ativar as etapas de aprovação, a equipe de marketing deve definir revisores individuais:

* A função de revisor do Adobe Campaign em uma atividade de aprovação pode ser um único revisor (Operador) ou um grupo de revisores (função Operador).
* Para permitir que os desenvolvedores de campanha selecionem os revisores como aprovadores em uma campanha ou entrega, os revisores e os grupos de revisores devem ser configurados no Adobe Campaign por um administrador.

## Configuração de aprovações {#configuring-approvals}

1. [Configurar aprovações para campanhas](/help/process-management/create-approvals-and-validation-workflows/configure-approvals-for-campaigns.md): se houver o mesmo conjunto de revisores para todas as entregas no fluxo de trabalho da campanha, aplique a funcionalidade de aprovação, configurando aprovações e revisores no nível da campanha. As tarefas de aprovação e os revisores são encaminhados para cada atividade de entrega do fluxo de trabalho depois que ele for executado.
2. [Configurar aprovações para entregas](/help/process-management/create-approvals-and-validation-workflows/configure-approvals-for-deliveries.md): também é possível configurar aprovações no nível da entrega. Se as etapas de aprovação de entrega e os revisores forem diferentes das etapas de aprovação da campanha e seus revisores, as configurações de entrega substituirão as configurações da campanha.
3. [Criar um processo de aprovação em um fluxo de trabalho](/help/process-management/create-approvals-and-validation-workflows/create-approval-process-in-a-workflow.md): a atividade de aprovação permite a criação de um processo de aprovação dentro de um fluxo de trabalho. Dessa forma, a lógica de seleção de direcionamento pode ser aprovada antes que a entrega seja iniciada. Ela também permite a aprovação em vários níveis no fluxo de trabalho, se necessário.

Para obter mais informações, consulte a [documentação](https://experienceleague.adobe.com/docs/campaign-classic/using/automating-with-workflows/flow-control-activities/approval.html?lang=pt-BR).
