---
title: Configurer Microsoft Forms
ms.author: jokay
author: dumptruckjon
manager: kathyl
audience: Admin
ms.topic: how-to
ms.service: forms-pro
ms.localizationpriority: high
description: Découvrez comment les administrateurs Microsoft 365 peuvent contrôler la façon dont Microsoft Forms est utilisé dans leur organisation. Découvrez également les réponses aux questions de sécurité et de conformité, telles que l’emplacement de stockage des données pour Microsoft Forms.
ms.openlocfilehash: abee1557f379f646b277866f32fc0640c0b643cd
ms.sourcegitcommit: 09bdc82ce67e74495b6c58d9c842e31c17956fc3
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/12/2021
ms.locfileid: "60951465"
---
# <a name="set-up-microsoft-forms"></a>Configurer Microsoft Forms


## <a name="overview"></a>[Vue d’ensemble](#tab/overview)

Microsoft Forms permet à vos utilisateurs de créer rapidement et facilement des questionnaires personnalisés, des enquêtes, des questionnaires, des inscriptions, etc. Lorsque vous créez un questionnaire ou un formulaire, vous pouvez inviter d'autres personnes à y répondre via n'importe quel navigateur web, voire sur des appareils mobiles. Une fois les résultats envoyés, vous pouvez utiliser des analyses intégrées pour évaluer les réponses. Les données de formulaire, comme les résultats d'un quiz, peuvent être exportées facilement vers Excel pour une évaluation ou une analyse plus approfondie.

Pour en savoir plus, reportez-vous à [Microsoft Form](https://support.microsoft.com/office/what-is-microsoft-forms-6b391205-523c-45d2-b53a-fc10b22017c8) Ou consultez notre [billet de blog Microsoft 365](https://go.microsoft.com/fwlink/?linkid=852256) sur Microsoft Forms.

>[!Note]
>Microsoft Forms est généralement disponible pour les clients Office 365 Éducation, les clients Microsoft 365 Apps for business et les clients disposant d'un compte Microsoft (Windows Live Hotmail, Live ou Outlook.com).

:::image type="content" source="./media/set-up-forms-team-event.png" alt-text="Afficher un aperçu à quoi ressemblera un formulaire sur un appareil mobile.":::

## <a name="configure"></a>[Configurer](#tab/configure)

Les administrateurs Microsoft 365 peuvent contrôler la façon dont Microsoft Forms est utilisé dans leur organisation via les tâches suivantes :

<table>
<thead>
<tr class="header">
<th><strong>Tâche d’administrateur</strong></th>
<th><strong>Description</strong></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><strong>Désactiver ou activer Microsoft Forms</strong></td>
<td>Microsoft Forms est activé par défaut pour votre organisation. Mais vous pouvez le<a href="https://support.microsoft.com/office/turn-off-or-turn-on-microsoft-forms-8dcbf3ab-f2d6-459a-b8be-8d9892132a43">désactiver</a> à tout moment.</td>
</tr>
<tr class="even">
<td><strong>Désactiver Microsoft Forms pour les membres individuels de votre organisation</strong></td>
<td>Lorsque vous désactivez Microsoft Forms pour une personne spécifique, elle ne pourra pas l’utiliser et la vignette <strong>Forms</strong> ne s’affichera pas pour elle dans le lanceur d’applications Microsoft 365 ou la page d’accueil.  Découvrez comment <a href="https://support.microsoft.com/office/turn-off-or-turn-on-microsoft-forms-8dcbf3ab-f2d6-459a-b8be-8d9892132a43">désactiver des formulaires pour des personnes spécifiques</a>. </td>
</tr>
<tr class="odd">
<td><strong>Configurer l’accès conditionnel Azure Active Directory Domain Services pour Microsoft Forms</strong></td>
<td><p>Pour configurer une stratégie d’accès conditionnel pour Microsoft Forms, consultez <a href="/azure/active-directory/conditional-access/">Documentation sur l’accès conditionnel Azure AD sur l’accès conditionnel</a> et incluez <strong>Microsoft Form</strong> dans les attributions d’<strong>Applications cloud</strong>.</p>
<p><strong>Note : </strong>Si les utilisateurs de votre organisation sont toujours bloqués même après avoir configuré l’accès conditionnel pour Microsoft Forms, assurez-vous que l’accès à Microsoft Office SharePoint Online et Exchange Online a également été accordé via l’accès conditionnel. <a href="/azure/active-directory/conditional-access/conditional-access-for-exo-and-spo">En savoir plus</a>.</p></td>
</tr>
<tr class="even">
<td><strong>Contrôler les paramètres de partage externe, enregistrer les noms des personnes de votre organisation et/ou protéger les formulaires contre le hameçonnage</strong></td>
<td><p>Dans le Centre d’administration Microsoft 365, vous pouvez :</p>
<ul>
<li><p>Contrôlez si les utilisateurs externes sont autorisés à collaborer avec des utilisateurs de votre organisation sur un formulaire ou un questionnaire.</p></li>
<li><p>Choisissez de capturer ou non les noms des personnes de votre organisation qui remplissent des formulaires.</p></li>
<li><p>Désactivez ou activez la détection automatique de l’hameçonnage sur les formulaires.</p></li>
</ul>
<p>En savoir plus sur ces <a href="https://support.microsoft.com/office/administrator-settings-for-microsoft-forms-48161c55-fbae-4f37-8951-9e3befc0248b">paramètres d’administrateur</a>.</p></td>
</tr>
<tr class="odd">
<td><strong>En permettre aux utilisateurs d’insérer un formulaire dans PowerPoint</strong></td>
<td><ol type="1">
<li><p>Connectez-vous à <a href="https://admin.microsoft.com/">https://admin.microsoft.com</a>.</p></li>
<li><p>Cliquez sur <strong>Paramètres</strong> &gt; <strong>Paramètres</strong>.</p></li>
<li><p>Dans la page <strong>Paramètres</strong>, sous l’onglet <strong>Services</strong>, cliquez sur <strong>Applications et services détenus par l’utilisateur</strong>..</p></li>
<li><p>Cochez l’option <strong>Autoriser l’utilisateur à accéder à l’Office Store</strong>, pour permettre aux utilisateurs d’insérer un formulaire dans PowerPoint.</p></li>
</ol>
<blockquote>
<p>N’oubliez pas que l’application de la modification peut prendre quelques heures. <a href="/office365/admin/manage/manage-deployment-of-add-ins>Learn more</a>.</p>
</blockquote></td>
</tr>
</tbody>
</table>


## <a name="security--compliance"></a>[Sécurité et conformité](#tab/security)

Si vous recherchez des informations concernant les normes juridiques, réglementaires et techniques en matière de sécurité du contenu et d’utilisation des données, cette section s’adresse à vous.

**Où les données sont-elles stockées pour Microsoft Forms ?**

Les données Microsoft Forms sont stockées sur des serveurs du États-Unis et de l’Europe. Toutes les données se trouvent aux États-Unis, à l’exception des locataires basés en Europe qui ont commencé à utiliser Microsoft Forms après mai 2017. Leurs données sont stockées dans des bases de données en Europe.

**Microsoft Forms est-il conforme?**

Microsoft Forms répond aux exigences de conformité RGPD depuis mai 2018. Pour plus d’informations, consultez [Demandes de la personne concernée dans Microsoft365 pour le RGPD](/microsoft-365/compliance/gdpr-dsr-office365?toc=/microsoft-365/enterprise/toc.json).

**Les protections de la loi fédérale FERPA et BAA sont-elles en place?**

Microsoft Forms répond aux normes de protection[FERPA](https://www.microsoft.com/trustcenter/compliance/ferpa) et de [l’accord d’association commerciale (BAA)](https://www.microsoft.com/TrustCenter/Compliance/HIPAA).

*Existe-t-il une limite au nombre d’utilisateurs et à la quantité de données stockées pour les comptes d’utilisateurs même après avoir quitté mon organisation ?*

Actuellement, il n’existe aucune limite au nombre d’utilisateurs pour lesquels les données sont conservées, tant que la mise en service de leurs comptes est dans le cadre du contrat de service en ligne de votre organisation. Il n’existe pas non plus de limite pour la quantité de données stockées pour les comptes d’utilisateurs.

*Le propriétaire d’origine d’un formulaire n’est plus dans mon organisation et/ou sa licence Microsoft Forms a été supprimée, donc qu’arrive-t-il aux données associées au formulaire qu’ils ont créé ?*

Toutes les données liées au compte seront supprimées 30 jours après la suppression d’un compte d’utilisateur de votre client (Azure AD).

## <a name="faq"></a>FAQ

**À quoi puis-je utiliser Microsoft Forms?**

Microsoft Forms est une application simple et légère qui vous permet de créer facilement des enquêtes, des questionnaires et des sondages. Dans les établissements d’enseignement, il peut être utilisé pour créer des questionnaires, recueillir des commentaires d’enseignants et de parents, ou planifier des activités de classe et de personnel. Dans les organisations commerciales, il peut être utilisé pour recueillir les commentaires des clients, mesurer la satisfaction des employés, améliorer votre produit ou votre entreprise, ou organiser des événements d’entreprise.

**Qui peut utiliser Microsoft Teams?**

L’utilisation de Microsoft Forms est gratuite pour toute personne disposant d’un compte Microsoft (Windows Live Hotmail, Live ou Outlook.com). Les clients Office 365 Éducation et applications Microsoft 365 Apps for business suivants peuvent également utiliser Microsoft Forms :

Office 365 Éducation

  - Office 365 A1 Plus

  - Office 365 A5

  - Clients existants ayant acheté Microsoft Office 365 pour l’éducation E3 avant sa mise hors service

Applications Microsoft 365 pour les entreprises

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

Votre avis nous intéresse\! Pour envoyer des commentaires sur Microsoft Forms, accédez au coin supérieur droit de votre formulaire et sélectionnez **Autres paramètres du formulaire** ![ Bouton autres options](./media/image2.png)\> **Commentaires**.

>[!Note]
>Pour en savoir plus, consultez [ Questions fréquentes sur Microsoft Forms](https://support.microsoft.com/office/frequently-asked-questions-about-microsoft-forms-495c4242-6102-40a0-add8-df05ed6af61c).

