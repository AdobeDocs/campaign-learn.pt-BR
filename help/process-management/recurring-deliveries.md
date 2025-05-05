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
source-git-commit: 4d21755204c22fbeb4ac3a2916e9ee68cd2e0f9a
workflow-type: ht
source-wordcount: '233'
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

>[!VIDEO](https://video.tv.adobe.com/v/3446879?quality=12&learn=on&captions=por_br){transcript=true}

## Como configurar uma entrega contínua {#how-to-set-up-a-continuous-delivery}

Este vídeo mostra como configurar uma entrega contínua com um query incremental.

>[!VIDEO](https://video.tv.adobe.com/v/3444572?quality=12&learn=on&captions=por_br){transcript=true}
