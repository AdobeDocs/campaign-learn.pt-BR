---
title: Solução de problemas do Painel de controle do Campaign
description: Saiba como solucionar problemas do Painel de controle do Campaign
feature: Painel de controle do Campaign
kt: 8520
doc-type: article
activity: use
team: PM
role: Admin
level: Experienced
source-git-commit: f8ed9264e592f4adf070a517049e3d36fc3112d5
workflow-type: tm+mt
source-wordcount: '340'
ht-degree: 19%

---

# Solução de problemas do [!UICONTROL Painel de controle do Campaign]

Saiba como solucionar problemas do Painel de controle do Campaign.

## Login e página inicial

### Sintoma: Não é possível iniciar sessão no Experience Cloud

**O que fazer:**
O usuário deve localizar a ID organizacional IMS (xxx). O Administrador deve adicionar o usuário ao Perfil de produto &quot;Campaign-xxx-Admins&quot; para cada instância que ele quiser gerenciar. Se o usuário for um administrador de todas as instâncias, ele deverá se adicionar como usuário.

### Sintoma: Os links na página inicial do Experience Cloud para acessar o [!UICONTROL Painel de controle] não aparecem para um usuário

**Causa:**
Os usuários não veem os links até que sejam adicionados como usuários ao Perfil do produto  _Campanha-xxx-Administradores/Admin_.

**O que fazer:**
O Administrador deve adicionar o usuário ao Perfil de produto  _Campaign-xxx-_  Adminspara cada instância que ele quiser gerenciar. Se o usuário for um administrador de todas as instâncias, ele deverá se adicionar como usuário.

### Sintoma: Uma Instância não está listada no [!UICONTROL Painel de Controle]

**Causa:**
Provavelmente, o usuário deve ser adicionado como um Perfil  ** userProduct  _Campaign-xxx-Administrators/_ Adminpara a instância que estiver ausente

**O que fazer:**
O Administrador deve adicionar o usuário ao Perfil de produto  _Campaign-xxx-_  Adminspara cada instância que ele quiser gerenciar. Se o usuário for um administrador de todas as instâncias, ele deverá se adicionar como &quot;usuários&quot;.

### Vídeos úteis

>[!VIDEO](https://video.tv.adobe.com/v/27183?quality=12)

*Verificar IMS Org ID (00:26 min)*

>[!VIDEO](https://video.tv.adobe.com/v/27147?quality=12)

*Como adicionar um administrador aos administradores do perfil do produto para usar o  [!UICONTROL Painel de controle do Campaign]  (01:03 min)*

### Documentação útil

* [Conheça o Painel de controle do Campaign](https://experienceleague.adobe.com/docs/control-panel/using/control-panel-home.html?lang=pt-BR)
* [Gerenciamento de permissões para o  [!UICONTROL Painel de controle do Campaign]](https://experienceleague.adobe.com/docs/control-panel/using/control-panel-home.html?lang=en)

## Estabelecer conexão com o servidor SFTP (cliente ou API)

A conexão com servidores SFTP requer:

* [!UICONTROL Permitir ] listar o endereço IP a partir do qual você está se conectando ao servidor SFTP
* Par de chave privada/pública que deve ser registrado no Adobe Campaign
* Para se conectar diretamente ao servidor SFTP, você também precisa de software cliente SFTP

### Documentação útil {#helpful-docs}

* [Fazer logon no servidor SFTP](https://experienceleague.adobe.com/docs/control-panel/using/control-panel-home.html?lang=en)
