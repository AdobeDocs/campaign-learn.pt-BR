---
title: Criar workflows de validação
description: Saiba como configurar diferentes fluxos de trabalho de validação de aprovação.
feature: Fluxos de trabalho, Aprovações
kt: 7991
doc-type: feature video
activity: setup
team: TM
role: Business Practitioner
level: Experienced
source-git-commit: f6bb16306773a4b6ff7aa390a514e9b31fe047d6
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 0%

---


# Criar workflows de validação

O Adobe Campaign oferece várias opções para que os profissionais de marketing revisem e forneçam conteúdo de entrega, direcionamento da campanha, extração de dados e aprovações de orçamento.

Este tutorial explica como configurar diferentes workflows de validação de aprovação.

## Pré-requisito {#prerequisite}

Antes de ativar as etapas de aprovação, a equipe de marketing deve definir revisores individuais:

* A função de revisor da Adobe Campaign em uma atividade de aprovação pode ser um único revisor (Operador) ou um grupo de revisores (função Operador).
* Para permitir que os desenvolvedores de campanha selecionem os revisores como aprovadores em uma campanha ou delivery, os revisores e os grupos de revisores devem ser configurados no Adobe Campaign por um administrador.

## Configuração de aprovações para campanhas {#configuring-approvals-for-campaigns}

Se você tiver o mesmo conjunto de revisores para todos os deliveries no workflow da campanha, aplique a funcionalidade de aprovação da campanha, configurando aprovações e revisores no nível da campanha. As tarefas de aprovação e os revisores são encaminhados para cada atividade de delivery do workflow depois que o workflow é executado.

>[!VIDEO](https://video.tv.adobe.com/v/25175?quality=12)

## Configuração de aprovações para deliveries {#configuring-approvals-for-deliveries}

Você também pode configurar aprovações em um nível de delivery. Se as etapas de aprovação de delivery e os revisores forem diferentes das etapas de aprovação da campanha e dos revisores, as configurações de delivery substituirão as configurações da campanha.

>[!VIDEO](https://video.tv.adobe.com/v/25176?quality=12)

## Configurar uma atividade de aprovação {#configuring-an-approval-activity}

Diferente das aprovações de delivery ou campanha, a atividade de aprovação permite criar um processo de aprovação em um workflow. Dessa forma, a lógica de seleção de target pode ser aprovada antes que o delivery seja iniciado. Ela também permite a aprovação em vários níveis no fluxo de trabalho, se necessário.

>[!VIDEO](https://video.tv.adobe.com/v/25174?quality=12)

Para obter mais informações, consulte a [Documentação de aprovação](https://experienceleague.adobe.com/docs/campaign-classic/using/automating-with-workflows/flow-control-activities/approval.html)
