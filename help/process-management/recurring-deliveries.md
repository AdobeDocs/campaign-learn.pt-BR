---
title: Como configurar campanhas de email recorrentes e contínuas
description: Saiba como configurar um delivery recorrente e contínuo e compreender as diferenças entre as duas abordagens.
feature: Workflows
kt: 7982
doc-type: feature video
activity: use
team: TM
role: Business Practitioner
level: Beginner
source-git-commit: 7609aa35dba225a05c8f5e3d3f75f4b6023772a0
workflow-type: tm+mt
source-wordcount: '239'
ht-degree: 21%

---


# Como configurar campanhas de email recorrentes e contínuas

Este tutorial explica como configurar um delivery recorrente e contínuo e as diferenças entre as duas abordagens.

## Rastreamento de entrega recorrente e contínua {#recurring-and-continuous-delivery-tracking}

Os deliveries recorrentes e contínuos diferem na maneira como os dados de contato são gerenciados:

* O **delivery contínuo** permite adicionar novos recipients a um delivery existente, o que evita a necessidade de criar um delivery toda vez que um novo recipient for adicionado. Você pode atualizar o anúncio diretamente no fluxo de trabalho da campanha e ele atualiza o template na pasta de recursos do template do delivery.

   Um delivery contínuo cria um ÚNICO delivery e logs de delivery (broadLog) e logs de rastreamento, que fazem referência a um delivery, são adicionados a cada execução.

![Delivery contínuo](/help/assets/delivery_continuous.jpg)

* Um **delivery recorrente** cria uma instância de delivery toda vez que é executado. Por exemplo, se o workflow estiver programado para ser executado uma vez por semana, o resultado será 52 deliveries em um ano. Também significa que o log abrangente e os logs de rastreamento são separados por instância de delivery.

![Delivery recorrente](/help/assets/delivery_recurring.jpg)

## Como configurar uma entrega recorrente {#how-to-set-up-a-recurring-delivery}

O vídeo explica como configurar um delivery recorrente e uma atividade de scheduler.

>[!VIDEO](https://video.tv.adobe.com/v/25040?quality=12)

## Como configurar uma entrega contínua {#how-to-set-up-a-continuous-delivery}

Este vídeo mostra como configurar um delivery contínuo com um query incremental.

>[!VIDEO](https://video.tv.adobe.com/v/25039?quality=12)
