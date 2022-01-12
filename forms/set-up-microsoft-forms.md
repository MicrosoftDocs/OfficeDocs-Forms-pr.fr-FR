---
title: Configurer Microsoft Forms
ms.author: jokay
author: dumptruckjon
manager: kathyl
audience: Admin
ms.topic: how-to
ms.service: microsoft-365-education
ms.localizationpriority: high
description: Découvrez comment les administrateurs Microsoft 365 peuvent contrôler la façon dont Microsoft Forms est utilisé dans leur organisation. Découvrez également les réponses aux questions de sécurité et de conformité, telles que l’emplacement de stockage des données pour Microsoft Forms.
ms.openlocfilehash: bb0e1a6ba8e2085550eb18a8bb393b34b197fe51
ms.sourcegitcommit: 80aa5565b4008855be844e8e5ab3f2779fba9a83
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/05/2022
ms.locfileid: "61723722"
---
# <a name="set-up-microsoft-forms"></a>Configurer Microsoft Forms

## <a name="overview"></a>Vue d’ensemble

Microsoft Forms permet à vos utilisateurs de créer rapidement et facilement des questionnaires personnalisés, des enquêtes, des questionnaires, des inscriptions, etc. Lorsque vous créez un questionnaire ou un formulaire, vous pouvez inviter d'autres personnes à y répondre via n'importe quel navigateur web, voire sur des appareils mobiles. Une fois les résultats envoyés, vous pouvez utiliser des analyses intégrées pour évaluer les réponses. Les données de formulaire, comme les résultats d'un quiz, peuvent être exportées facilement vers Excel pour une évaluation ou une analyse plus approfondie.

Pour en savoir plus, reportez-vous à [Microsoft Form](https://support.microsoft.com/office/what-is-microsoft-forms-6b391205-523c-45d2-b53a-fc10b22017c8) Ou consultez notre [billet de blog Microsoft 365](https://go.microsoft.com/fwlink/?linkid=852256) sur Microsoft Forms.

>[!Note]
>Microsoft Forms est généralement disponible pour les clients Office 365 Éducation, les clients Microsoft 365 Apps for business et les clients disposant d'un compte Microsoft (Windows Live Hotmail, Live ou Outlook.com).

:::image type="content" source="./media/set-up-forms-team-event.png" alt-text="Afficher un aperçu à quoi ressemblera un formulaire sur un appareil mobile.":::

## <a name="configure"></a>Configurer

Les administrateurs Microsoft 365 peuvent contrôler la façon dont Microsoft Forms est utilisé dans leur organisation via les tâches suivantes :

|Tâche d’administrateur   |Description   |
|----------|-----------|
|**Désactiver ou activer Microsoft Forms**|Microsoft Forms est activé par défaut pour votre organisation. Mais vous pouvez le[désactiver](turn-off-turn-on-microsoft-forms.md) à tout moment.|
|**Désactiver Microsoft Forms pour les membres individuels de votre organisation**|Lorsque vous désactivez Microsoft Forms pour une personne spécifique, elle ne pourra pas l’utiliser et la vignette *Forms* ne s’affichera pas pour elle dans le lanceur d’applications Microsoft 365 ou la page d’accueil. Découvrez comment [désactiver des formulaires pour des personnes spécifiques](turn-off-turn-on-microsoft-forms.md).|
|**Configurer l’accès conditionnel Azure Active Directory Domain Services pour Microsoft Forms**|Pour configurer une stratégie d’accès conditionnel pour Microsoft Forms, consultez [Documentation sur l’accès conditionnel Azure AD sur l’accès conditionnel](/azure/active-directory/conditional-access) et incluez *Microsoft Form* dans les attributions d’*Applications cloud*. <br/><br/> **Note : **Si les utilisateurs de votre organisation sont toujours bloqués même après avoir configuré l’accès conditionnel pour Microsoft Forms, assurez-vous que l’accès à Microsoft Office SharePoint Online et Exchange Online a également été accordé via l’accès conditionnel. [En savoir plus](/azure/active-directory/conditional-access/block-legacy-authentication).|
|**Contrôler les paramètres de partage externe, enregistrer les noms des personnes de votre organisation et/ou protéger les formulaires contre le hameçonnage**|Dans le Centre d’administration Microsoft 365, vous pouvez : <ul><li>Contrôlez si les utilisateurs externes sont autorisés à collaborer avec des utilisateurs de votre organisation sur un formulaire ou un questionnaire.</li><li>Choisissez de capturer ou non les noms des personnes de votre organisation qui remplissent des formulaires.</li><li>Désactivez ou activez la détection automatique de l’hameçonnage sur les formulaires.</li></ul><br/>En savoir plus sur ces [paramètres d’administrateur](administrator-settings-microsoft-forms.md).|
|**En permettre aux utilisateurs d’insérer un formulaire dans PowerPoint**|<ol><li>Connectez-vous à https://admin.microsoft.com.</li><li>Cliquez sur **Paramètres** > **Paramètres**.</li><li>Dans la page **Paramètres**, sous l’onglet **Services**, cliquez sur **Applications et services détenus par l’utilisateur**..</li><li>Cochez l’option **Autoriser l’utilisateur à accéder à l’Office Store**, pour permettre aux utilisateurs d’insérer un formulaire dans PowerPoint.</li></ol><br/>N’oubliez pas que l’application de la modification peut prendre quelques heures. [En savoir plus](/microsoft-365/admin/manage/manage-deployment-of-add-ins)|

## <a name="security--compliance"></a>Sécurité et conformité

Si vous recherchez des informations concernant les normes juridiques, réglementaires et techniques en matière de sécurité du contenu et d’utilisation des données, cette section s’adresse à vous.

**Où les données sont-elles stockées pour Microsoft Forms ?**

Les données Microsoft Forms sont stockées sur des serveurs du États-Unis et de l’Europe. Toutes les données se trouvent aux États-Unis, à l’exception des locataires basés en Europe qui ont commencé à utiliser Microsoft Forms après mai 2017. Leurs données sont stockées dans des bases de données en Europe.

**Microsoft Forms est-il conforme?**

Microsoft Forms répond aux exigences de conformité RGPD depuis mai 2018. Pour plus d’informations, accédez à [Microsoft 365 Demandes des personnes concernées pour le RGPD.](/microsoft-365/compliance/gdpr-dsr-office365?toc=/microsoft-365/enterprise/toc.json)

**Les protections de la loi fédérale FERPA et BAA sont-elles en place?**

Microsoft Forms répond aux normes de protection[FERPA](https://www.microsoft.com/trustcenter/compliance/ferpa) et de [l’accord d’association commerciale (BAA)](https://www.microsoft.com/TrustCenter/Compliance/HIPAA).

**Existe-t-il une limite au nombre d’utilisateurs et à la quantité de données stockées pour les comptes d’utilisateurs même après avoir quitté mon organisation ?**

Actuellement, il n’existe aucune limite au nombre d’utilisateurs pour lesquels les données sont conservées, tant que la mise en service de leurs comptes est dans le cadre du contrat de service en ligne de votre organisation. Il n’existe pas non plus de limite pour la quantité de données stockées pour les comptes d’utilisateurs.

**Le propriétaire d’origine d’un formulaire n’est plus dans mon organisation et/ou sa licence Microsoft Forms a été supprimée, donc qu’arrive-t-il aux données associées au formulaire qu’ils ont créé ?**

Toutes les données liées au compte seront supprimées 30 jours après la suppression d’un compte d’utilisateur de votre client (Azure AD).

## <a name="faq"></a>FAQ

**À quoi puis-je utiliser Microsoft Forms?**

Microsoft Forms est une application simple et légère qui vous permet de créer facilement des enquêtes, des questionnaires et des sondages. Dans les établissements d’enseignement, il peut être utilisé pour créer des questionnaires, recueillir des commentaires d’enseignants et de parents, ou planifier des activités de classe et de personnel. Dans les organisations commerciales, il peut être utilisé pour recueillir les commentaires des clients, mesurer la satisfaction des employés, améliorer votre produit ou votre entreprise, ou organiser des événements d’entreprise.

**Qui peut utiliser Microsoft Teams?**

L’utilisation de Microsoft Forms est gratuite pour toute personne disposant d’un compte Microsoft (Windows Live Hotmail, Live ou Outlook.com). Les clients Office 365 Éducation et applications Microsoft 365 Apps for business suivants peuvent également utiliser Microsoft Forms :

**Office 365 Éducation**

  - Office 365 A1 Plus

  - Office 365 A5

  - Clients existants ayant acheté Microsoft Office 365 pour l’éducation E3 avant sa mise hors service

**Microsoft 365 Apps for business**

  - Microsoft 365 Business Basic

  - Microsoft 365 Business Standard

  - Microsoft 365 Business Premium

  - Applications Microsoft 365 for entreprise

  - Microsoft 365 Entreprise plans E1, E3 et E5

  - Clients Office 365 Entreprise E4 existants qui ont acheté E4 avant sa mise hors service

Connectez-vous à [forms.office.com](https://forms.office.com/) et commencez à créer des enquêtes, des questionnaires et des sondages.

**Une personne sans compte Microsoft 365 soumet toujours une enquête ou un questionnaire sur Microsoft Forms?**

Les auteurs sur Microsoft Forms peuvent activer/désactiver leurs paramètres pour permettre aux utilisateurs extérieurs à leur organisation de répondre à leur enquête ou questionnaire. Dans ce cas, les utilisateurs soumettront des réponses de manière anonyme. Si vous souhaitez savoir qui a répondu à votre enquête ou questionnaire, vous pouvez demander aux personnes interrogées de remplir leurs noms dans le cadre de votre questionnaire.

**Quelle est la limite du nombre de formulaires pouvant être créés et du nombre de réponses qu’un formulaire peut recevoir ?**

Les clients Office 365 Éducation et applications Microsoft 365 Apps for business peuvent créer jusqu’à 200 formulaires et chaque formulaire peut recevoir jusqu’à 50 000 réponses. Les utilisateurs de Microsoft Forms disposant d’un compte Microsoft (Windows Live Hotmail, Live ou Outlook.com) peuvent créer jusqu’à 200 formulaires et chaque formulaire peut recevoir jusqu’à 1 000 réponses pour les comptes payants et jusqu’à 200 réponses pour les comptes gratuits. En savoir plus sur les limites des [formulaires, questions, réponses, et les caractère dans Forms](https://support.microsoft.com/office/form-question-response-and-character-limits-in-microsoft-forms-ec15323d-92a4-4c33-bf88-3fdb9e5b5fea).

Si vous avez besoin d’autres réponses, nous vous recommandons d’exporter des réponses existantes vers un classeur Excel, puis de les effacer de votre enquête ou questionnaire. Cela vous permettra de collecter plus de réponses une fois effacé.

**Ce que les navigateurs web utilisent Microsoft Forms?**

Microsoft Forms est optimisé pour Internet Explorer 11, Edge, Chrome (dernière version), Firefox (dernière version), Chrome sur Android (dernière version) et Safari sur iOS (dernière version).

**Dans quelles langues Microsoft Forms sont disponibles ?**

Consultez les [langues prises en charge](https://support.microsoft.com/office/languages-supported-by-microsoft-forms-c17498cb-cbf6-4178-ae83-bd24934398ac) et les [paramètres de langue](https://support.microsoft.com/office/language-settings-for-microsoft-forms-b282f9aa-0fe4-4290-b1e1-827a8a35ac27) pour Microsoft Forms.

**Microsoft Forms remplacera-t-il Microsoft InfoPath?**

Non. Microsoft InfoPath a été une solution pour créer des formulaires personnalisables qui peuvent activer des flux de travail automatisés, tandis que Microsoft Forms est une application simple et légère permettant de collecter rapidement des informations via des enquêtes et des questionnaires.

Microsoft InfoPath est remplacé par les listes Microsoft Office SharePoint Online Flow et PowerApps solutions modernes pour numériser les formulaires d’entreprise traditionnels, automatiser les flux de travail et transformer les processus métier. [En savoir plus](https://products.office.com/business/business-process-automation).

**Où puis-je déposer des commentaires, pour signaler des bugs ou formuler des demandes de fonctionnalité par exemple?**

Nous voulons connaître votre avis ! Pour envoyer des commentaires sur Microsoft Forms, accédez au coin supérieur droit de votre formulaire et sélectionnez **Autres paramètres du formulaire** ![Bouton autres options](./media/image2.png) > **Commentaires**.

> [!Note]
> Pour en savoir plus, consultez [ Questions fréquentes sur Microsoft Forms](https://support.microsoft.com/office/frequently-asked-questions-about-microsoft-forms-495c4242-6102-40a0-add8-df05ed6af61c).

