---
title: Examiner et débloquer les formulaires ou les utilisateurs détectés et bloqués pour un hameçonnage potentiel
ms.author: jokay
author: dumptruckjon
manager: kathyl
audience: Admin
ms.topic: how-to
ms.service: forms-pro
ms.localizationpriority: high
description: Microsoft Forms permet aux révisions automatiques de l’ordinateur de détecter de manière proactive la collecte de données sensibles malveillantes dans les formulaires et les enquêtes. Si vous êtes administrateur général et/ou de sécurité, vous pouvez vous connecter au Centre d’administration Microsoft 365 pour examiner et débloquer les formulaires détectés et bloqués en cas d’hameçonnage potentiel et d’intention malveillante.
ms.openlocfilehash: dd4b92c09393db4c81ac5e7711ee7331ac35558e
ms.sourcegitcommit: 09bdc82ce67e74495b6c58d9c842e31c17956fc3
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/12/2021
ms.locfileid: "60951500"
---
# <a name="review-and-unblock-forms-or-users-detected-and-blocked-for-potential-phishing"></a>Examiner et débloquer les formulaires ou les utilisateurs détectés et bloqués pour un hameçonnage potentiel

Dans Microsoft Forms, nous activons les révisions automatiques sur les ordinateurs pour détecter de manière proactive la collection malveillante de données sensibles dans les formulaires et empêcher temporairement ces formulaires de collecter des réponses. En savoir plus sur [Microsoft Forms et la prévention proactive de l’hameçonnage](https://support.microsoft.com/office/microsoft-forms-and-proactive-phishing-prevention-b3950a20-296d-4e8e-96f5-594ced998a90).

>[!Note]
>Les étapes décrites dans ce document s’appliquent également à [Dynamics 365 Customer Voice](https://go.microsoft.com/fwlink/p?linkid=2128500) (anciennement Forms Pro). Notez qu’une licence Dynamics 365 Customer Voice est nécessaire pour débloquer les enquêtes Dynamics 365 Customer Voice. [En savoir plus](/dynamics365/customer-voice/help-hub).

## <a name="review-alerts-in-the-microsoft-365-defender-portal"></a>Examiner des alertes dans le portail Microsoft 365 Defender

Si vous êtes administrateur général ou de sécurité, vous recevrez des alertes dans le portail [Microsoft 365 Defender](https://security.microsoft.com/) concernant les formulaires d’hameçonnage potentiels pour lesquels vous pouvez prendre des mesures.

>[!Note]
> Si vous êtes administrateur général, vous recevrez des messages de confidentialité des données pour votre organisation, y compris des notifications quotidiennes de tout formulaire créé au sein de votre locataire qui a été détecté et bloqué en cas d’hameçonnage potentiel. Ces notifications s’affichent dans le [Centre de messages](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter) de **Notifications d’hameçonnage de Microsoft Forms **. (Si vous ne voyez pas cette notification dans l’onglet/affichage**Tous les messages actifs**, vous pouvez la trouver dans l’onglet/affichage **Messages ignorés**.) Pour chaque notification, sélectionnez le lien **URL de révision de l’administrateur de formulaires** pour passer en revue les formulaires bloqués.  
  
Pour que les administrateurs de sécurité reçoivent également des notifications sur les formulaires d’hameçonnage potentiels, les administrateurs généraux doivent leur attribuer le rôle de[Lecteur de confidentialité du Centre de messages](/azure/active-directory/roles/permissions-reference#message-center-privacy-reader). Pour en savoir plus sur le Centre de messages, consultez les[questions fréquemment posées](/microsoft-365/admin/manage/message-center). Découvrez également comment [définir les préférences de courrier pour les messages de confidentialité des données](/microsoft-365/admin/manage/message-center#preferences).

1.  Connectez-vous au portail [Microsoft 365 Defender](https://security.microsoft.com/).

2.  Sélectionnez **Incidents & alertes** \> **Alertes**. Vous pouvez voir une ou l’ensemble des alertes suivantes pour les formulaires :
    
      - **L’utilisateur ne peut pas partager de formulaires et collecter des réponses**.
    
      - **Formulaire marqué d'un indicateur et confirmé comme hameçonnage**
    
      - **Formulaire bloqué en raison d’une tentative d’hameçonnage potentielle**

3.  Sélectionnez une alerte pour l’examiner. Pour passer en revue le formulaire marqué d’un indicateur, appuyez ou cliquez sur les trois points dans le coin inférieur droit en regard du bouton **Gérer l’alerte**, puis sélectionnez **Réviser ce formulaire**.
 
    :::image type="content" source="./media/review-unblock-forms-review-this-form.png" alt-text="Réviser cette option de formulaire":::

    >[!Tip]
    >En savoir plus sur les [stratégies d’alertes dans Microsoft 365](/microsoft-365/compliance/alert-policies).

## <a name="unblock-a-form-or-confirm-its-phishing-attempt"></a>Débloquer un formulaire ou confirmer sa tentative d’hameçonnage

Pour chaque formulaire que vous examinez, vous pouvez choisir de le débloquer ou de confirmer le hameçonnage.

### <a name="unblock"></a>Débloquer

Sélectionnez **Débloquer** si vous ne pensez pas qu’un formulaire a une intention malveillante.

>[!Note]
>Si une personne de votre locataire vous demande de débloquer son formulaire, nous vous suggérons de demander des informations de formulaire spécifiques (par exemple, date et heure de blocage, titre) afin d’identifier plus efficacement la notification dans le Centre d’administration. Dans la mesure où les notifications sont envoyées quotidiennement et incluent tous les formulaires détectés au cours des dernières 24 heures, les informations d’identification du formulaire sont utiles.

### <a name="confirm-phishing"></a>Confirmer l’hameçonnage

Sélectionnez **Confirm phishing** si vous pensez qu’un formulaire a une intention malveillante. Le formulaire sera bloqué définitivement et son propriétaire ne pourra plus le modifier ou le supprimer.

Une fois que vous avez sélectionné **Confirmer l’hameçonnage**, cliquez ou appuyez sur ** supprimer le formulaire** pour supprimer définitivement le formulaire de votre locataire. Nous vous suggérons vivement de réinitialiser immédiatement le mot de passe d’un compte de votre locataire qui, selon vous, a été compromis.

>[!Tip]
>Votre sélection de **Confirmer l’hameçonnage**permet Microsoft Forms d’améliorer la précision de sa détection. 

## <a name="commonly-asked-questions"></a>Forum aux questions

**Si j’accède à la révision d’un formulaire bloqué, pourquoi ne vois-je pas d’options pour le débloquer ou confirmer le hameçonnage ?**

Lors de la révision, vous pouvez voir qu’un bloc pour un formulaire a déjà été levé. Cela signifie qu’entre le moment où un formulaire a été bloqué et le moment où vous l’avez examiné, le propriétaire du formulaire a supprimé les mots clés marqués pour hameçonnage potentiel. Dans ce scénario, aucune autre action de votre part n’est requise.

**Si un formulaire a été bloqué pour hameçonnage confirmé, puis-je le supprimer ?**

Si le formulaire a déjà été bloqué pour hameçonnage confirmé, sélectionnez **Supprimer le formulaire** pour le supprimer de votre locataire.

**Que se passe-t-il si je n’effectue aucune action sur un formulaire bloqué ?**

Si vous choisissez de ne pas prendre d’action (débloquer un formulaire ou confirmer son intention d’hameçonnage), le formulaire reste bloqué. Le propriétaire du formulaire peut toujours modifier le formulaire et supprimer les mots clés qui ont été marqués pour hameçonnage potentiel.

**Que dois-je modifier ou supprimer le contenu bloqué dans le formulaire ?**

Si vous préférez modifier et/ou supprimer le contenu bloqué, vous pouvez générer une page de co-édition et gérer le formulaire en tant que co-auteur. Pour ce faire, cliquez sur le lien **ouvrez une page de co-édition** situé dans la messagerie au-dessus du formulaire que vous examinez.

## <a name="remove-restrictions-for-blocked-microsoft-forms-users"></a>Supprimer les restrictions pour les utilisateurs Microsoft Forms bloqués

Microsoft Forms bloque les utilisateurs qui ont tenté à plusieurs reprises de collecter des informations personnelles ou sensibles à partir de la distribution de formulaires et de la collecte de réponses. Les administrateurs généraux seront avertis de ces utilisateurs bloqués via le [Centre de messages](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter). Si vous pensez qu’un utilisateur bloqué n’a aucune intention malveillante et que son compte est sécurisé, vous pouvez effectuer les étapes suivantes pour les débloquer.

>[!Note]
>Les administrateurs de sécurité peuvent également recevoir des notifications sur les formulaires d’hameçonnage potentiels une fois qu’un administrateur général leur a attribué le rôle [Lecteur de confidentialité du Centre de messages](/azure/active-directory/roles/permissions-reference#message-center-privacy-reader).

1.  Accédez au [Centre de messages](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter)et recherchez la notification, **Prevent/Fix: Microsoft Forms détection d’hameçonnage potentiel**.

    >[!Note]
    >Si vous ne voyez pas cette notification dans la **Tous les messages actifs** onglet/affichage, vous pouvez la trouver dans l’onglet/affichage **Messages ignorés**.
 
    Cette notification contient une liste d’utilisateurs de votre locataire qui ne peuvent pas partager de formulaires et collecter des réponses.

2.  Cliquez sur le lien fourni dans la notification pour passer en revue les utilisateurs bloqués.

3.  Pour chaque utilisateur que vous pensez n’avoir aucune intention malveillante, vous pouvez choisir de cliquer sur le lien **Débloquer**dans la colonne**Actions** associée à cet utilisateur.

    >[!Note]
    >Si vous pensez qu’un utilisateur a une intention malveillante, aucune autre action de votre part n’est requise.

    >[!Note]
    >L’opération peut prendre jusqu’à 30 minutes avant la suppression des restrictions.

