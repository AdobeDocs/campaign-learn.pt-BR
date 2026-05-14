---
title: Criar entregas de email recorrentes e contínuas
description: Saiba como configurar uma entrega recorrente e contínua e compreender as diferenças entre as duas abordagens.
feature: Workflows
jira: KT-7982
thumbnail: 342637.jpg
doc-type: feature video
activity: use
team: TM
role: User
level: Intermediate
exl-id: 469aecd7-4774-42c6-b07f-82792dfdc9c2
TQID: https://experienceleague.adobe.com/pdYTRO3rBq3BdS-WUGcx3POKjD6V4lH1dco4W9L6FwM
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
source-git-commit: 1f6ccc9f0e59ce16a4e781d2d366cf0257b1c8aa
workflow-type: tm+mt
source-wordcount: 233
ht-degree: 100%

---

# Criar entregas de email recorrentes e contínuas

Este tutorial explica como configurar uma entrega recorrente e contínua e as diferenças entre as duas abordagens.

## Rastreamento de entrega recorrente e contínua {#recurring-and-continuous-delivery-tracking}

As entregas recorrentes e contínuas diferem na maneira como os dados de contato são gerenciados:

* A **entrega contínua** permite adicionar novos destinatários a uma entrega existente, o que evita a criação de uma nova entrega cada vez que um novo destinatário é adicionado. Você pode atualizar o criativo diretamente no fluxo de trabalho da campanha e ele atualizará o modelo na pasta Recursos do template da entrega.

  Uma entrega contínua criará uma ÚNICA entrega. Logs do delivery (broadLog) e logs de rastreamento que fazem referência a uma entrega serão adicionados a cada execução.

![Entrega contínua](/help/assets/delivery_continuous.jpg)

* Uma **entrega recorrente** cria uma instância de entrega sempre que é executada. Por exemplo, se o fluxo de trabalho estiver programado para ser executado uma vez por semana, o resultado será 52 entregas em um ano. Também significa que o log abrangente e os logs de rastreamento serão separados por cada instância da entrega.

![Entrega recorrente](/help/assets/delivery_recurring.jpg)

## Como configurar uma entrega recorrente {#how-to-set-up-a-recurring-delivery}

Este vídeo explica como configurar uma entrega recorrente e uma atividade de scheduler.

>[!VIDEO](https://video.tv.adobe.com/v/342638?quality=12&learn=on){transcript=true}

## Como configurar uma entrega contínua {#how-to-set-up-a-continuous-delivery}

Este vídeo mostra como configurar uma entrega contínua com uma consulta incremental.

>[!VIDEO](https://video.tv.adobe.com/v/342637?quality=12&learn=on){transcript=true}
