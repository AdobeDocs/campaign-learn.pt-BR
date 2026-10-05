---
title: Introdução a notificações por push para Android – Introdução
description: Este tutorial percorre as etapas envolvidas no envio de notificações por push do Adobe Campaign e no recebimento dessas notificações em aplicativos Android™.
feature: Push
jira: KT-6438
doc-type: article
activity: setup
team: TM
role: Admin, Developer
level: Experienced
recommendations: noCatalog
exl-id: 91ff4bae-8598-4227-b4c9-4e436ce7400d
TQID: 'https://experienceleague.adobe.com/llhU9-u6ri1njd6wSTE1CTZTmYerQDz7-R2WY4ahWzs'
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
  - id: d0e9f0b2-1f2b-4134-9844-49cd4e950f27
    internal-label: Campaign v8
feature_v2:
  - id: a4671286-a59f-47e3-b97b-90627a1977d5
    internal-label: Communication channels
subfeature_v2:
  - id: a4657621-810c-498b-8a27-7ced9c176dda
    internal-label: Push notifications
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
    internal-label: Developer
level_v2:
  - id: d378ca77-2da1-4f39-ad92-1917fe974a38
    internal-label: Experienced
topic_v2:
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
    internal-label: Personalization
source-git-commit: 369f9c3691b6326e521ebc9139aac1d2ee7c3ce2
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 100%
---
# Introdução a notificações por push para Android – Introdução

O Adobe Campaign permite enviar notificações [!DNL push] personalizadas e segmentadas para [!DNL iOS] e dispositivos móveis [!DNL Android™]. Este tutorial guiará você pelas etapas relativas ao envio de [!DNL push] notificações do Adobe Campaign para um aplicativo [!DNL Android™].

## Pré-requisitos

Antes de começar, você deve ter o seguinte:

1) **Aplicativo para dispositivos móveis Android™**

   Este tutorial não apresenta as etapas detalhadas necessárias para configurar o aplicativo para dispositivos móveis. Você deve ter um aplicativo para dispositivos móveis **[!DNL Android™]com o [!DNL Campaign SDK] integrado**.

   Você pode encontrar uma descrição detalhada das etapas necessárias na documentação do produto:

   [Integração do SDK do Campaign no aplicativo para dispositivos móveis](https://experienceleague.adobe.com/pt-br/docs/campaign-classic/using/sending-messages/sending-push-notifications/integrating-campaign-sdk-into-the-mobile-application)

2) Pacote **[!DNL Mobile App channel]instalado**

   O pacote [!DNL Mobile App channel] deve estar instalado na instância do [!DNL Campaign]. O vídeo a seguir explica como verificar se o [!DNL Mobile App channel] está instalado em sua instância e como instalá-lo, caso ele ainda não esteja instalado.

>[!VIDEO](https://video.tv.adobe.com/v/326544?quality=12&learn=on){transcript=true}

## Visão geral do tutorial

Gostaríamos de enviar uma notificação promocional personalizada do [!DNL push] para os assinantes do aplicativo móvel [!DNL Neotrip] [!DNL Android™]. O aplicativo [!DNL Neotrip] é configurado com o [!DNL Campaign SDK] e o [!DNL Mobile App channel] é ativado na instância do [!DNL Campaign].

As seguintes etapas de configuração são obrigatórias:

### Etapa 1: estenda o esquema de assinatura do aplicativo para personalizar notificações do [!DNL push]

Para personalizar a notificação [!DNL push], primeiro você deve [estender o esquema de subscrição do aplicativo](/help/tutorial-get-started-with-push-notifications-for-android/extend-the-app-subscription-schema.md). Isso permite que o sistema armazene os valores de personalização que são recebidos do aplicativo quando o usuário se inscreve no serviço.

### Etapa 2: configure o serviço Android™ e crie o aplicativo para dispositivos móveis no Campaign

Em seguida, [o serviço Android™ deve ser configurado e o aplicativo para dispositivos móveis criado no Campaign](/help/tutorial-get-started-with-push-notifications-for-android/configure-an-android-service-in-campaign.md). Nesta etapa, o aplicativo [!DNL Neotrip] é definido como o destino da notificação por push.

### Etapa 3: configure e envie a notificação por push

Agora, a notificação por push está pronta para ser [configurada e enviada](/help/tutorial-get-started-with-push-notifications-for-android/configure-and-send-push-notifications.md).

## Iniciar o tutorial

Etapa 1: [estenda o esquema de assinatura do aplicativo](/help/tutorial-get-started-with-push-notifications-for-android/extend-the-app-subscription-schema.md)
