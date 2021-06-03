---
title: Introdução a notificações por push para Android – Introdução
description: Este tutorial o orienta pelas etapas envolvidas no envio de notificações por push da Adobe Campaign e no recebimento dessas notificações em seu aplicativo Android™.
feature: Push
kt: 6438
doc-type: article
activity: setup
team: TM
role: Administrator, Developer
level: Experienced
source-git-commit: 39bed2fe5fbe19101a9684b29d73f61026ad77b2
workflow-type: tm+mt
source-wordcount: '318'
ht-degree: 41%

---

# Introdução a notificações por push para Android – Introdução

O Adobe Campaign permite enviar notificações [!DNL push] personalizadas e segmentadas para [!DNL iOS] e dispositivos móveis [!DNL Android™]. Este tutorial o orienta pelas etapas envolvidas no envio de [!DNL push] notificações do Adobe Campaign para um aplicativo [!DNL Android™].

## Pré-requisitos

Antes de começar, você deve ter o seguinte:

1) **Aplicativo móvel Android™**

   Este tutorial não apresenta as etapas detalhadas necessárias para configurar o aplicativo para dispositivos móveis. Você deve ter um aplicativo móvel **[!DNL Android™]com o [!DNL Campaign SDK] integrado**.

   Você pode encontrar uma descrição detalhada das etapas necessárias na documentação do produto:

   [Integração do SDK do Campaign no aplicativo para dispositivos móveis](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/sending-push-notifications/integrating-campaign-sdk-into-the-mobile-application.html?lang=pt-BR)

2) Pacote **[!DNL Mobile App channel]instalado**

   O pacote [!DNL Mobile App channel] deve ser instalado na instância [!DNL Campaign]. O vídeo a seguir explica como verificar se o [!DNL Mobile App channel] está instalado em sua instância e como instalá-lo, caso ele ainda não esteja instalado.

>[!VIDEO](https://video.tv.adobe.com/v/326544?quality=12)

## Visão geral do tutorial

O objetivo é enviar uma notificação promocional personalizada [!DNL push] aos assinantes do [!DNL Neotrip] [!DNL Android™] aplicativo móvel. O aplicativo [!DNL Neotrip] é configurado com o [!DNL Campaign SDK] e o [!DNL Mobile App channel] é ativado na instância [!DNL Campaign].

As seguintes etapas de configuração são obrigatórias:

### Etapa 1: estenda o esquema de assinatura do aplicativo para personalizar notificações do [!DNL push]

Para personalizar a notificação [!DNL push], primeiro você deve [estender o schema de assinatura do aplicativo](/help/tutorial-get-started-with-push-notifications-for-android/extend-the-app-subscription-schema.md). Isso permite que o sistema armazene os valores de personalização que são recebidos do aplicativo quando o usuário se inscreve no serviço.

### Etapa 2: Configure o serviço Android™ e crie o aplicativo móvel no Campaign

Em seguida, [o serviço Android™ deve ser configurado e o aplicativo móvel criado no Campaign](/help/tutorial-get-started-with-push-notifications-for-android/configure-an-android-service-in-campaign.md). Nesta etapa, o aplicativo [!DNL Neotrip] é definido como o destino da notificação por push.

### Etapa 3: configure e envie a notificação por push

Agora, a notificação por push está pronta para ser [configurada e enviada](/help/tutorial-get-started-with-push-notifications-for-android/configure-and-send-push-notifications.md).

## Iniciar o tutorial

Etapa 1: [estenda o esquema de assinatura do aplicativo](/help/tutorial-get-started-with-push-notifications-for-android/extend-the-app-subscription-schema.md)
