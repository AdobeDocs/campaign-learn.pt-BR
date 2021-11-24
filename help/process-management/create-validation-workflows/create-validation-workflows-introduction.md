---
title: Criar workflows de validação - Introdução
description: Saiba como configurar diferentes workflows de validação de aprovação.
feature: Workflows, Approvals
doc-type: feature video
activity: setup
team: TM
role: User
level: Experienced
exl-id: fa4c2180-15bb-424b-a54e-c7d744385fb6
source-git-commit: f25e3e7553d23aacf96c0f05e1ad78ee783192ff
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 66%

---

# Criar workflows de validação - Introdução

O Adobe Campaign oferece várias opções para que os profissionais de marketing revisem e forneçam conteúdo de entrega, direcionamento da campanha, extração de dados e aprovações de orçamento.

## Pré-requisito {#prerequisite}

Antes de ativar as etapas de aprovação, a equipe de marketing deve definir revisores individuais:

* A função de revisor do Adobe Campaign em uma atividade de aprovação pode ser um único revisor (Operador) ou um grupo de revisores (função Operador).
* Para permitir que os desenvolvedores de campanha selecionem os revisores como aprovadores em uma campanha ou entrega, os revisores e os grupos de revisores devem ser configurados no Adobe Campaign por um administrador.

## Configuração de aprovações {#configuring-approvals}

O Campaign oferece três níveis diferentes para aprovações:

1. [Configurar aprovações para campanhas](/help/process-management/create-validation-workflows/configure-approvals-for-campaigns.md): Se você tiver o mesmo conjunto de revisores para todos os deliveries no workflow da campanha, aplique a funcionalidade de aprovação da campanha, configurando aprovações e revisores no nível da campanha. As tarefas de aprovação e os revisores são encaminhados para cada atividade de entrega do fluxo de trabalho depois que o fluxo de trabalho é executado.
2. [Configurar aprovações para deliveries](/help/process-management/create-validation-workflows/configure-approvals-for-deliveries.md): Você também pode configurar aprovações em um nível de delivery. Se as etapas de aprovação de entrega e os revisores forem diferentes das etapas de aprovação da campanha e dos revisores, as configurações de entrega substituirão as configurações da campanha.
3. [Criar um processo de aprovação em um workflow](/help/process-management/create-validation-workflows/create-approval-process-in-a-workflow.md): A atividade de aprovação permite a criação de um processo de aprovação em um workflow. Dessa forma, a lógica de seleção de direcionamento pode ser aprovada antes que a entrega seja iniciada. Ela também permite a aprovação em vários níveis no fluxo de trabalho, se necessário.

Para obter mais informações, consulte [documentação](https://experienceleague.adobe.com/docs/campaign-classic/using/automating-with-workflows/flow-control-activities/approval.html?lang=pt-BR).
