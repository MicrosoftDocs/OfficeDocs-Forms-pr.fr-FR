---
title: Informations de l’administrateur
ms.author: jokay
author: dumptruckjon
manager: kathyl
audience: Admin
ms.topic: how-to
ms.service: forms-pro
ms.localizationpriority: high
description: Cet article répond aux questions les plus fréquemment posées sur les informations d’administrateur de Microsoft Forms.
ms.openlocfilehash: 3fed9f104b6a44a7c23221b204796b22c8fb5109
ms.sourcegitcommit: 09bdc82ce67e74495b6c58d9c842e31c17956fc3
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/12/2021
ms.locfileid: "60951488"
---
# <a name="admin-information"></a>Informations de l’administrateur

## <a name="getting-started"></a>Prise en main

**Comment puis-je désactiver ou activer Microsoft Forms ?**

Par défaut, Microsoft Forms est activé pour tous le monde dans une organisation. Les administrateurs informatiques Microsoft 365 peuvent désactiver Microsoft Forms dans le Centre d’administration Microsoft 365, sous l’onglet **Gestion des utilisateurs**. Consultez [Configurer Microsoft Forms](set-up-microsoft-forms.md) et [Désactiver Microsoft Forms](turn-off-turn-on-microsoft-forms.md) pour obtenir plus d’informations.

**Comment faire pour autoriser l’accès à Microsoft Forms pour des personnes spécifiques de mon organisation uniquement ?**

Les administrateurs peuvent modifier les autorisations d’accès pour des personnes spécifiques de l’organisation. Consultez [Paramètres d’administrateur dans Microsoft Forms](administrator-settings-microsoft-forms.md).

## <a name="data-storage"></a>Stockage des données

**Où les données sont-elles stockées pour Microsoft Forms ?**

Les données Microsoft Forms sont stockées sur des serveurs aux États-Unis, à l’exception des données pour les clients basés en Europe. Les données des locataires basés en Europe sont stockées sur des serveurs en Europe.

## <a name="user-activity"></a>Activité utilisateur

**Comment puis-je voir les activités effectuées dans Microsoft Forms par des personnes de mon organisation ?**

Vous pouvez consulter les [activités de Microsoft Forms](/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance?view=o365-worldwide#microsoft-forms-activities) dans le journal d'audit du[Centre de sécurité Microsoft 365](https://security.microsoft.com/?rfr=OfficeScc). En savoir plus sur [l’audit dans Office 365 (pour les administrateurs)](https://support.microsoft.com/topic/auditing-in-office-365-for-admins-9f6484d2-0fd2-17de-165f-c41346023906).

## <a name="user-account-information"></a>Informations sur le compte d’utilisateur

**Comment puis-je vérifier si un compte d’utilisateur a été « supprimé définitivement » ?**

1. Les administrateurs peuvent se connecter à [Microsoft Graph](https://developer.microsoft.com/graph/graph-explorer).

2. Dans la zone de recherche supérieure, collez l’URL suivante :

   `https://graph.microsoft.com/v1.0/directory/deletedItems/microsoft.graph.user?$filter=mail eq '*user email*'`

   >[!Note]
   >*e-mail de l’utilisateur* = adresse de messagerie du propriétaire du formulaire qui a quitté votre organisation et/ou dont le compte a été désactivé.

3. Cliquez sur**Exécuter la requête**.

Si les informations du compte que vous recherchez sont renvoyées dans votre requête, cela signifie que le compte a été supprimé de façon réversible et se trouve dans la limite de 30 jours. Un administrateur global peut transférer les formulaires appartenant au compte supprimé (suppression possible) à l’aide de la méthode de transfert décrite précédemment.

Si les informations du compte que vous recherchez ne sont pas renvoyées dans votre requête, cela signifie que le compte existe toujours dans le client Office 365 ou a été supprimé il y a plus de 30 jours. Si le compte existe ou est dans l’état désactivé dans le client Office 365, un administrateur global peut transférer les formulaires dont il est propriétaire. Si le compte a été « supprimé définitivement » du client Office 365, un administrateur global ne sera pas en mesure de transférer les formulaires détenus par ce compte. Ces formulaires ne sont pas non plus récupérables.

**Existe-t-il une limite au nombre d’utilisateurs et à la quantité de données stockées pour les comptes d’utilisateurs même après avoir quitté mon organisation ?**

Actuellement, il n’existe aucune limite au nombre d’utilisateurs pour lesquels les données sont conservées, tant que la mise en service de leurs comptes est dans le cadre du contrat de service en ligne de votre organisation. Il n’existe pas non plus de limite pour la quantité de données stockées pour les comptes d’utilisateurs.

**Qu’advient-il des données d’un formulaire si la licence Microsoft Forms du propriétaire a été supprimée, ou si l’utilisateur est désactivé ou supprimé de votre client (Azure AD) ?**

Si la licence du propriétaire a été supprimée ou si son compte est désactivé, la quantité de données stockées pour le compte d’utilisateur n’est pas changée.

Si un compte d’utilisateur a été supprimé de votre client (Azure AD), toutes les données liées au compte seront supprimées 30 jours après la suppression de l’utilisateur.

## <a name="form-ownership-transfer"></a>Transfert de propriété du formulaire

**Le propriétaire d’origine d’un formulaire n’est plus dans mon organisation. Comment puis-je transférer la propriété de son formulaire ?**

Pour transférer la forme d’une personne qui a quitté votre organisation, les conditions suivantes doivent être remplies :

  - Vous êtes l’administrateur général de l’organisation et vous avez une licence de Forms valide.

  - L’employé dont vous souhaitez transférer le formulaire possède un compte qui a été supprimé ou désactivé.

  - Le formulaire est transféré dans les 30 jours suivant la suppression d’un compte.

> [!Note]
> Il n’existe aucune restriction de temps pour transférer la propriété d’un formulaire à partir d’un compte qui a été désactivé (et non supprimé).

1. Si toutes les conditions sont remplies, vous pouvez transférer la propriété du formulaire. Dans la barre d’adresses de votre navigateur, remplacez l’URL existante par ce qui suit :

    `https://forms.office.com/Pages/delegatepage.aspx? originalowner=\[*email address*\]`

   >[!Note]
   >*e-mail de l’utilisateur* = adresse de messagerie du propriétaire du formulaire qui a quitté votre organisation et/ou dont le compte a été désactivé.
   > Par exemple, si le propriétaire du formulaire («Jason Fabian ») a quitté votre organisation (« Contoso »), votre URL de contournement ressemblerait à ceci : `https://forms.office.com/Pages/delegatepage.aspx?originalowner=JasonFabian@contoso.com`

2. Vous avez désormais accès aux formulaires de l’ancien employé. Dans le formulaire que vous souhaitez transférer, cliquez sur le **Autres actions du formulaire**![bouton Plus d’options](./media/image2.png), puis sélectionnez **Déplacer**.

   >[!Note]
   >Si vous essayez de transférer la propriété du formulaire à un employé actif au sein de votre organisation, vous pouvez le déplacer vers un groupe à qui il appartient. Si vous n’êtes pas déjà membre de ce groupe, vous devez le rejoindre pour effectuer le transfert. Une fois le transfert de propriété du formulaire terminé, vous pouvez choisir de quitter le groupe.

**Lorsque j’essaie de transférer la propriété d’un formulaire, pourquoi reçois-je une erreur ?**

Si vous recevez un message d’erreur, l’un des messages suivants peut vous empêcher de transférer la propriété :

|Message d’erreur|Explication|
| --- | --- |
| ***Nous ne pouvons pas accéder à cette page***<br/><br/>Le propriétaire du formulaire&#39; possède toujours un compte actif. | Le propriétaire du formulaire dispose toujours d’une licence et d’un compte Forms actifs. |
| ***Nous ne pouvons pas accéder à cette page***<br/><br/>Assurez-vous que&#39;avez entré l’adresse e-mail correctement et que le compte du propriétaire des formulaires&#39;pas été supprimé il y a plus de 30 jours. | L’adresse e-mail est incorrectement orthographée et/ou le compte du propriétaire des formulaires a été supprimé il y a plus de 30 jours. |
| ***Nous ne pouvons pas accéder à cette page***<br/><br/>Assurez-vous que&#39;avez entré l’adresse e-mail correctement, puis essayez à nouveau. | L’adresse e-mail est manquante ou mal orthographiée. |

## <a name="forms-usage-in-outlook-or-powerpoint"></a>Utilisation des formulaires dans Outlook ou PowerPoint

**Les membres de mon organisation ne sont pas en mesure d’ajouter un Sondage à un message électronique Outlook. Comment puis-je résoudre ce problème ?**

Le paramètre**d’authentification moderne** pour Outlook doit être activé pour garantir que les membres de votre organisation puissent [créer un sondage dans Outlook](https://support.microsoft.com/office/create-a-poll-in-outlook-46893563-ab12-4bd0-aff7-26f5a488fea0).

1. Connectez-vous [https://admin.microsoft.com](https://admin.microsoft.com/) avec votre compte scolaire ou professionnel.

2. Sélectionnez **Paramètres** \> **Paramètres de l’organisation**.

   >[!Note]
   > Si vous ne voyez pas l’option **Paramètres**, sélectionnez le ![bouton Plus d’options](./media/image2.png)**Afficher tout** dans le volet gauche.

3.  Sélectionnez **Authentification moderne**.

4.  Cochez l’option ,**Activer l’authentification moderne pour Outlook 2013 pour Windows et versions ultérieures (recommandé)**

En savoir plus sur [l’authentification multi-facteur](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication?view=o365-worldwide) et moderne, et comment la configurer et la déployer au sein de votre organisation.

**Je ne souhaite pas déployer de compléments Office pour l’ensemble de mon organisation. Les membres de mon organisation peuvent-ils toujours utiliser le complément Forms pour PowerPoint ?**

Oui, vous pouvez utiliser le [Déploiement centralisé](/office/dev/add-ins/publish/centralized-deployment) pour déployer uniquement le complément Forms pour PowerPoint.

1.  Connectez-vous [https://admin.microsoft.com](https://admin.microsoft.com/) avec votre compte scolaire ou professionnel.

2.  Sélectionnez **Paramètres** \> **Compléments**.

    >[!Note]
    >Si vous ne voyez pas l’option **Paramètres**, sélectionnez le ![ bouton Plus d’options](./media/image2.png)**Afficher tout** dans le volet gauche.

3.  Dans la liste des **Compléments**, sélectionnez **Formulaires**.

4.  Sous **Attribuer des utilisateurs** dans le volet **Modifier les formulaires**, sélectionnez **Tout le monde**.

5.  Sélectionnez **Enregistrer**.


## <a name="forms-and-anti-phishing"></a>Forms et anti-hameçonnage

**Que puis-je faire à propos de l’hameçonnage et de l’intention malveillante potentielle dans les formulaires au sein de mon client ?**

Dans Microsoft Forms, nous activons les révisions automatiques sur les ordinateurs pour détecter de manière proactive la collection malveillante de données sensibles dans les formulaires et empêcher temporairement ces formulaires de collecter des réponses.

En savoir plus sur [Microsoft Forms et la prévention proactive de l’hameçonnage](https://support.microsoft.com/office/microsoft-forms-and-proactive-phishing-prevention-b3950a20-296d-4e8e-96f5-594ced998a90).

Si vous êtes un administrateur général et/ou de sécurité, vous pouvez vous connecter au centre d'administration Microsoft 365 à [admin.microsoft.com](https://admin.microsoft.com/) et aller au [Centre de messages](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter). Ici, vous obtiendrez un résumé quotidien de tous les formulaires bloqués. Pour chaque formulaire répertorié, vous pouvez choisir de le débloquer ou de confirmer sa tentative d’hameçonnage. En savoir plus sur la façon d’[examiner et de débloquer les formulaires ou les utilisateurs détectés et bloqués pour un hameçonnage potentiel](review-unblock-forms-users-detected-blocked-potential-phishing.md).
