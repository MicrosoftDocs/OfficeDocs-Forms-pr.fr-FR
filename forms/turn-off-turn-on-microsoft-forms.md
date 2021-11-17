---
title: Désactiver ou activer Microsoft Forms
ms.author: jokay
author: dumptruckjon
manager: kathyl
audience: Admin
ms.topic: how-to
ms.service: forms-pro
ms.localizationpriority: high
description: Cet article explique comment l’administrateur Microsoft 365 peuvent désactiver ou activer Microsoft Forms pour l’ensemble de leur organisation ou des personnes spécifiques de leur organisation.
ms.openlocfilehash: 2d1280bd7d61dc8b31cfb84dfeaced2662603e4f
ms.sourcegitcommit: 09bdc82ce67e74495b6c58d9c842e31c17956fc3
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/12/2021
ms.locfileid: "60951459"
---
# <a name="turn-off-or-turn-on-microsoft-forms"></a>Désactiver ou activer Microsoft Forms

Par défaut, [Microsoft Forms](https://support.microsoft.com/office/what-is-microsoft-forms-6b391205-523c-45d2-b53a-fc10b22017c8) est activé pour tout le monde dans votre organisation. Si vous êtes un [administrateur](https://support.microsoft.com/topic/eac4d046-1afd-4f1a-85fc-8219c79e1504), vous pouvez [configurer Microsoft Forms](https://support.microsoft.com/office/set-up-microsoft-forms-cc52287a-4550-464d-9a1b-457bf9df2240), puis le désactiver ou le réactiver pour l’ensemble de votre organisation ou uniquement pour des personnes spécifiques.

## <a name="turn-off-microsoft-forms-for-everyone-in-your-organization"></a>Désactiver Microsoft Forms pour tous les membres de votre organisation

1.  Connectez-vous à [Microsoft Azure](https://portal.azure.com/).

2.  Dans le volet gauche, cliquez sur **Azure Active Directory Domain Services**.

3.  Aller aux **Applications d’entreprise**.

4.  Naviguez vers les services requis, puis répétez les étapes 5 à 7 pour le **Type d’application** \> **CollabDBService** et les **applications Microsoft** \> **Microsoft Forms**.
    
      - Dans le champ de recherche sous la liste déroulante **Type d’application**, tapez **CollabDBService**. Sélectionnez **CollabDBService** dans la liste des résultats de recherche.
    
      - Dans la liste déroulante **Type d’application**, sélectionnez **Applications Microsoft**. Dans le champ de recherche sous la liste déroulante **Type d’application** liste déroulante, tapez **Microsoft Forms**, puis sélectionnez **Microsoft Forms** dans la liste des résultats de recherche.

5.  Sous **Gérer**, cliquez sur **Propriétés**.

6.  Pour l’option, **Activé pour que les utilisateurs se connectent ?**, sélectionnez **No**.

7.  Cliquez sur **Enregistrer**.

## <a name="turn-off-microsoft-forms-for-specific-people-in-your-organization"></a>Désactiver Microsoft Forms pour des personnes spécifiques de votre organisation

1.  Connectez-vous à Microsoft 365 avec votre compte professionnel ou scolaire en tant qu'administrateur général. [Découvrez comment vous connecter](https://support.microsoft.com/office/where-to-sign-into-microsoft-365-for-business-e9eb7d51-5430-4929-91ab-6157c5a050b4).

2.  Dans le Centre d’administration Microsoft365, cliquez sur **Utilisateurs** \> **Utilisateurs actifs**.

3.  Sélectionnez la zone en regard du nom de la personne pour laquelle vous souhaitez désactiver Microsoft Forms.

4.  Dans le ruban, cliquez sur **Gérer les licences de produit **.

5.  Dans le formulaire de compte qui s’ouvre, sous l’onglet **Licenses et applications**, développez la section Applications et faites défiler jusqu’à l’option Microsoft Forms. 

    :::image type="content" source="./media/turn-forms-off-on-licenses-apps.jpg" alt-text="Les options de compte dans le Centre d’Administration Microsoft 365":::

6.  Décochez la case pour désactiver Microsoft Forms. Pour l’activer, sélectionnez la case à cocher.

    :::image type="content" source="./media/turn-forms-off-on-plan-e1.jpg" alt-text="Bascule MicrosoftForms":::

     > [!Note]
     > [Vérifiez cette liste](https://support.microsoft.com/office/office-licenses-that-include-microsoft-forms-efa14679-5d99-47c5-bdf1-2fc838767f7e) pour voir si vous disposez d’une licence Office incluant Microsoft Forms. Si votre licence est répertoriée, vous devez désactiver la case à cocher Microsoft Forms pour désactiver complètement l’accès utilisateur.

7.  En bas de la liste **Applications**, cliquez sur **Enregistrer les modifications**.

## <a name="i-turned-on-microsoft-forms-but-people-in-my-organization-still-cant-access-it"></a>J’ai activé Microsoft Forms, mais les membres de mon organisation ne peuvent toujours pas y accéder

Vérifiez le paramètre suivant dans Microsoft Azure pour vous assurer que Microsoft Forms est activé :

1.  Connectez-vous à [Microsoft Azure](https://portal.azure.com/).

2.  Dans le volet gauche, cliquez sur **Azure Active Directory Domain Services**.

3.  Aller aux **Applications d’entreprise**.

4.  Naviguez vers les services requis, puis répétez les étapes 5 à 7 pour le **Type d’application** \> **CollabDBService** et les **applications Microsoft** \> **Microsoft Forms**.
    
      - Dans le champ de recherche sous la liste déroulante du **Type d’application**, tapez **CollabDBService**. Sélectionnez **CollabDBService** dans la liste des résultats de recherche.
    
      - Dans la liste déroulante **Type d’application**, sélectionnez **Applications Microsoft**. Dans le champ de recherche sous la liste déroulante **Type d’application** liste déroulante, tapez **Microsoft Forms**, puis sélectionnez **Microsoft Forms** dans la liste des résultats de recherche.

5.  Sous **Gérer**, cliquez sur **Propriétés**.

6.  Pour l’option, **Activé pour que les utilisateurs se connectent ?**, sélectionnez **Ouu**.

7.  Cliquez sur **Enregistrer**.

    >[!Note]
    >Les services Windows SharePoint Services doivent également être activés pour que les membres de votre organisation puissent accéder à Microsoft Forms.

## <a name="feedback-for-microsoft-forms"></a>Commentaires sur Microsoft Forms

Votre avis nous intéresse\! Pour envoyer des commentaires sur Microsoft Forms, accédez au coin supérieur droit de votre formulaire et sélectionnez **Autres paramètres du formulaire** ![ Bouton autres options](./media/image2.png) \> **Commentaires**.

