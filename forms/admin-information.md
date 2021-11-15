---
title: 管理者情報
ms.author: jokay
author: dumptruckjon
manager: kathyl
audience: Admin
ms.topic: how-to
ms.service: forms-pro
ms.localizationpriority: high
description: この記事では、Microsoft Forms の管理者情報についてよく寄せられる質問とその回答を紹介します。
ms.openlocfilehash: 3fed9f104b6a44a7c23221b204796b22c8fb5109
ms.sourcegitcommit: 09bdc82ce67e74495b6c58d9c842e31c17956fc3
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/12/2021
ms.locfileid: "60951566"
---
# <a name="admin-information"></a>管理者情報

## <a name="getting-started"></a>はじめに

**Microsoft Forms を有効または無効にするにはどうすればよいですか?**

既定では、組織内のすべてのユーザーに対して Microsoft Forms が有効になっています。 Microsoft 365 の IT 管理者は、Microsoft 365 管理センターの **[ユーザー管理]** タブで Microsoft Forms を無効にできます。詳細については、「[Microsoft Forms のセットアップ](set-up-microsoft-forms.md)」と「[Microsoft Forms を有効または無効にする](turn-off-turn-on-microsoft-forms.md)」を参照してください。

**組織内の特定のユーザーだけに Microsoft Forms へのアクセスを許可するにはどうすればよいですか?**

管理者は、組織内の特定のユーザーに対してアクセス許可を変更できます。 「[Microsoft Forms での管理者設定](administrator-settings-microsoft-forms.md)」を参照してください。

## <a name="data-storage"></a>データ ストレージ

**Microsoft Forms のデータはどこに保存されていますか?**

Microsoft Forms のデータは、欧州のテナントのデータを除き、米国のサーバーに保存されています。 欧州のテナントのデータは、欧州にあるサーバーに保存されています。

## <a name="user-activity"></a>ユーザー アクティビティ

**組織内のユーザーが Microsoft Forms で実行したアクティビティを確認するにはどうすればよいですか?**

[Microsoft Forms でのアクティビティ](/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance?view=o365-worldwide#microsoft-forms-activities)は、[Microsoft 365 セキュリティ センター](https://security.microsoft.com/?rfr=OfficeScc)監査ログで確認できます。 詳細については、「[Office 365 での監査 (管理者向け)](https://support.microsoft.com/topic/auditing-in-office-365-for-admins-9f6484d2-0fd2-17de-165f-c41346023906)」を参照してください。

## <a name="user-account-information"></a>ユーザー アカウント情報

**ユーザー アカウントが "物理的に削除" されたかどうかを確認するにはどうすればよいですか?**

1. 管理者は [Microsoft Graph](https://developer.microsoft.com/graph/graph-explorer) にログインできます。

2. 上部の検索ボックスに、次の URL を貼り付けます。

   `https://graph.microsoft.com/v1.0/directory/deletedItems/microsoft.graph.user?$filter=mail eq '*user email*'`

   >[!Note]
   >*ユーザーのメールアドレス* = 組織を離れたか、アカウントが無効になっているフォームの所有者のメール アドレス。

3. **[クエリの実行]** をクリックします。

目的のアカウント情報がクエリで返される場合は、アカウントが回復可能な削除によって削除され、30 日間の期限内であることを意味しています。 グローバル管理者は、前述の転送方法を使用して、回復可能な削除によって削除されたアカウントが所有するフォームを転送できます。

目的のアカウント情報がクエリで返されない場合は、アカウントが Office 365 テナントにまだ存在するか、削除されてから 30 日が経過していることを意味しています。 アカウントが存在するか、Office 365 テナントで無効な状態にある場合、グローバル管理者はアカウントが所有するフォームを転送できます。 アカウントが Office 365 テナントから "物理的に削除" された場合は、グローバル管理者は、そのアカウントが所有するフォームを転送できません。 また、これらのフォームを復元することはできません。

**ユーザーが組織を離れた後でも、ユーザー アカウントに保存されるユーザー数とデータ量に制限はありますか?**

現時点では、アカウントのプロビジョニングが組織のオンライン サービス契約の範囲内にある限り、データが保持されるユーザー数に制限はありません。 また、ユーザー アカウントに保存されるデータ量に制限はありません。

**所有者の Microsoft Forms ライセンスが削除された場合、またはユーザーが無効になったか、テナント (Azure AD) から削除された場合、フォームのデータはどうなりますか?**

所有者ライセンスが削除されたか、所有者のアカウントが無効になっている場合、ユーザー アカウントに保存されるデータ量に変更はありません。

ユーザー アカウントがテナント (Azure AD) から削除された場合、アカウント関連のすべてのデータは、ユーザーが削除された 30 日後に削除されます。

## <a name="form-ownership-transfer"></a>フォームの所有権の転送

**フォームの元の所有者が組織に所属しなくなりました。フォームの所有権を転送するにはどうすればよいですか?**

組織を離れたユーザーのフォームを転送するには、次の要件を満たす必要があります。

  - 組織のグローバル管理者であり、有効な Forms ライセンスを持っている。

  - フォームの転送元である従業員が、削除されたか無効になっているアカウントを持っている。

  - フォームが、アカウントが削除されて 30 日以内に転送される。

> [!Note]
> 無効になっている (削除されていない) アカウントからフォームの所有権を転送する場合、時間制限はありません。

1. すべての要件が満たされている場合は、フォームの所有権を転送できます。 ブラウザーのアドレス バーで、既存の URL を次に置き換えます。

    `https://forms.office.com/Pages/delegatepage.aspx? originalowner=\[*email address*\]`

   >[!Note]
   >*ユーザーのメールアドレス* = 組織を離れたか、アカウントが無効になっているフォームの所有者のメール アドレス。
   > たとえば、フォームの所有者 ("Jason Fabian") が組織 ("Contoso") を離れた場合、回避策 URL は次のようになります: `https://forms.office.com/Pages/delegatepage.aspx?originalowner=JasonFabian@contoso.com`

2. これで、以前の従業員のフォームにアクセスできます。 転送するフォームで、**[その他のフォームのアクション]**![[その他のオプション] ボタン](./media/image2.png)の順にクリックし、**[移動]** を選択します。

   >[!Note]
   >フォームの所有権を組織内の現在アクティブな従業員に転送しようとしている場合は、その従業員を所属するグループに移動できます。 自分がそのグループのメンバーではない場合は、転送を実行するためにそのグループに参加する必要があります。 フォームの所有権の転送が完了したら、グループから離れることを選択できます。

**フォームの所有権を転送しようとするときに、エラーが発生するのはなぜですか?**

エラー メッセージが表示される場合は、次の原因のいずれかによって所有権を転送できない場合があります。

|エラー メッセージ|説明|
| --- | --- |
| ***このページにはアクセスできません***<br/><br/>フォームの所有者は、まだアクティブなアカウントを持っています。 | フォームの所有者は、まだアクティブな Forms ライセンスとアカウントを持っています。 |
| ***このページにはアクセスできません***<br/><br/>メール アドレスが正しく入力され、フォームの所有者のアカウントが削除されてから 30 日以上が経過していないことを確認してください。 | メール アドレスのスペルが正しくないか、フォームの所有者のアカウントが削除されてから 30 日以上が経過しています。 |
| ***このページにはアクセスできません***<br/><br/>メール アドレスが正しく入力されていることを確認してから、もう一度やり直してください。 | メール アドレスが存在しないか、スペルが間違っています。 |

## <a name="forms-usage-in-outlook-or-powerpoint"></a>Outlook または PowerPoint での Forms の使用状況

**組織内のユーザーが Outlook メール メッセージに投票を追加できません。どうすればよいですか?**

組織内のユーザーが [Outlook で投票を作成する](https://support.microsoft.com/office/create-a-poll-in-outlook-46893563-ab12-4bd0-aff7-26f5a488fea0)には、Outlook の**先進認証**設定を有効にする必要があります。

1. 職場または学校のアカウントを使用して、[https://admin.microsoft.com](https://admin.microsoft.com/) にサインインします。

2. **[設定]** \> **[組織の設定]** の順に選択します。

   >[!Note]
   > **[設定]** オプションが表示されない場合、左側のウィンドウで ![[その他のオプション] ボタン > ](./media/image2.png)**[すべて表示]** の順に選択します。

3.  **[先進認証]** を選択します。

4.  **[Windows 用 Outlook 2013 以降の先進認証を有効にする (推奨)]** のオプションをオンにします。

先進認証と[多要素認証](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication?view=o365-worldwide)の詳細情報と、設定して組織に展開する方法について参照してください。

**Office アドインを組織全体には展開しない場合でも、組織内のユーザーが PowerPoint 用の Forms アドインを使用することはできますか?**

はい、[一元展開](/office/dev/add-ins/publish/centralized-deployment)を使用して、PowerPoint 用の Forms アドインだけを展開できます。

1.  職場または学校のアカウントを使用して、[https://admin.microsoft.com](https://admin.microsoft.com/) にサインインします。

2.  **[設定]** \> **[アドイン]** の順に選択します。

    >[!Note]
    >**[設定]** オプションが表示されない場合、左側のウィンドウで ![[その他のオプション] ボタン > ](./media/image2.png)**[すべて表示]** の順に選択します。

3.  **[アドイン]** リストで、**[フォーム]** を選択します。

4.  **[フォームの編集]** ウィンドウの **[ユーザーの割り当て]** で、**[すべてのユーザー]** を選択します。

5.  [**保存**] を選択します。


## <a name="forms-and-anti-phishing"></a>フォームとフィッシング詐欺対策

**テナント内のフォームでのフィッシング詐欺や潜在的な悪意のある攻撃に対処するにはどうすればよいですか?**

Microsoft Forms では、自動化されたマシン レビューにより、フォーム内の機密データの悪意のある収集を事前に検出し、それらのフォームによる応答の収集を一時的にブロックできます。

[Microsoft Forms および積極的なフィッシング詐欺の防止](https://support.microsoft.com/office/microsoft-forms-and-proactive-phishing-prevention-b3950a20-296d-4e8e-96f5-594ced998a90)の詳細情報を参照してください。

グローバル管理者またはセキュリティ管理者の場合は、[admin.microsoft.com](https://admin.microsoft.com/) で Microsoft 365 管理センターにログインして、[メッセージ センター](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter)に移動できます。 ここでは、すべてのブロックされたフォームの日次要約を取得できます。 一覧表示されているフォームごとに、ブロックを解除するか、フィッシング詐欺の試みを確認することを選択できます。 [フィッシング詐欺の可能性が検出されてブロックされたフォームまたはユーザーのレビューとブロック解除](review-unblock-forms-users-detected-blocked-potential-phishing.md)の方法の詳細を参照してください。
