---
title: Microsoft Forms のセットアップ
ms.author: jokay
author: dumptruckjon
manager: kathyl
audience: Admin
ms.topic: how-to
ms.service: forms-pro
ms.localizationpriority: high
description: Microsoft 365 管理者が組織での Microsoft Forms の使用方法を制御する方法について説明します。 また、Microsoft Forms のデータが保存されている場所など、セキュリティとコンプライアンスに関する質問に対する回答も紹介します。
ms.openlocfilehash: abee1557f379f646b277866f32fc0640c0b643cd
ms.sourcegitcommit: 09bdc82ce67e74495b6c58d9c842e31c17956fc3
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/12/2021
ms.locfileid: "60951535"
---
# <a name="set-up-microsoft-forms"></a>Microsoft Forms のセットアップ


## <a name="overview"></a>[概要](#tab/overview)

Microsoft Forms を使用すると、カスタマイズされたクイズ、調査、アンケート、登録、その他のものをすばやく簡単に作成できます。 クイズやフォームを作成する場合、どの Web ブラウザー (モバイル デバイス上でも) を使用している人にも回答してもらうように招待できます。 回答が提出されたら、組み込みの分析機能を使用して応答を評価することができます。 クイズ回答などのフォーム データは、さらに分析したりランク付けしたりするために Excel にエクスポートできます。

詳細については、「[Microsoft Forms とは](https://support.microsoft.com/office/what-is-microsoft-forms-6b391205-523c-45d2-b53a-fc10b22017c8)」を参照してください。 または、Microsoft Forms に関する [Microsoft 365 のブログ記事](https://go.microsoft.com/fwlink/?linkid=852256)を参照してください。

>[!Note]
>Microsoft Forms は通常、Office 365 Education のお客様、Microsoft 365 Apps for business のお客様、および Microsoft アカウント (Hotmail、Live、または Outlook.com) をお持ちのお客様にご利用いただけます。

:::image type="content" source="./media/set-up-forms-team-event.png" alt-text="モバイル デバイス上でのフォームの外観のプレビュー":::

## <a name="configure"></a>[構成](#tab/configure)

Microsoft 365 管理者は、次のタスクを通じて組織での Microsoft Forms の使用方法を制御することができます。

<table>
<thead>
<tr class="header">
<th><strong>管理タスク</strong></th>
<th><strong>Description</strong></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><strong>Microsoft Forms を有効または無効にする</strong></td>
<td>既定では、Microsoft Forms は組織に対して有効になっています。 いつでも<a href="https://support.microsoft.com/office/turn-off-or-turn-on-microsoft-forms-8dcbf3ab-f2d6-459a-b8be-8d9892132a43">無効</a>にできます。</td>
</tr>
<tr class="even">
<td><strong>組織内の個々のユーザーに対して Microsoft Forms を無効にする</strong></td>
<td>Microsoft Forms を何らかの理由で無効にした場合、そのユーザーは使用できず、<strong>[Forms]</strong> タイルが Microsoft 365 アプリ起動ツールまたはホームページで非表示になります。  <a href="https://support.microsoft.com/office/turn-off-or-turn-on-microsoft-forms-8dcbf3ab-f2d6-459a-b8be-8d9892132a43">特定のユーザーに対してフォームを無効にする</a>方法をご覧ください。 </td>
</tr>
<tr class="odd">
<td><strong>Microsoft Forms の Azure Active Directory の条件付きアクセスをセットアップする</strong></td>
<td><p>Microsoft Forms の条件付きアクセス ポリシーを設定するには、「<a href="/azure/active-directory/conditional-access/">Azure AD 条件付きアクセスのドキュメント</a>」を参照し、<strong>クラウド アプリ</strong>の割り当てに <strong>Microsoft Forms</strong> を含めます。</p>
<p><strong>注: </strong>Microsoft Forms の条件付きアクセスを設定した後も、組織内のユーザーが引き続きブロックされている場合は、条件付きアクセスで SharePoint Online と Exchange Online へのアクセスも許可されていることを確認してください。 <a href="/azure/active-directory/conditional-access/conditional-access-for-exo-and-spo">詳細情報</a> を参照してください。</p></td>
</tr>
<tr class="even">
<td><strong>外部共有設定の制御、組織内のユーザーの名前の記録、フィッシングからフォームを保護する</strong></td>
<td><p>Microsoft 365 管理センターでは、次のことを実行できます。</p>
<ul>
<li><p>外部ユーザーがフォームやクイズで組織内のユーザーと共同作業することを許可するかどうかを制御します。</p></li>
<li><p>フォームに入力する組織内のユーザーの名前をキャプチャするかどうかを選択します。</p></li>
<li><p>フォームでの自動フィッシング検出をオフまたはオンにします。</p></li>
</ul>
<p>これらの<a href="https://support.microsoft.com/office/administrator-settings-for-microsoft-forms-48161c55-fbae-4f37-8951-9e3befc0248b">管理設定</a>の詳細情報をご覧ください。</p></td>
</tr>
<tr class="odd">
<td><strong>ユーザーがフォームを PowerPoint に挿入できるようにする</strong></td>
<td><ol type="1">
<li><p>Sign in to <bpt id="p1">&lt;a href="https://admin.microsoft.com/"&gt;</bpt><ph id="ph1">https://admin.microsoft.com</ph><ept id="p1">&lt;/a&gt;</ept>.</p></li>
<li><p><strong>[設定]</strong> &gt; <strong>[設定]</strong> の順にクリックします。</p></li>
<li><p><strong>[設定]</strong> ページで、<strong>[サービス]</strong> タブから <strong>[ユーザーが所有するアプリとサービス]</strong> をクリックします。</p></li>
<li><p><strong>[ユーザーに Office ストアへのアクセスを許可する]</strong> のオプションをオンにして、ユーザーがフォームを PowerPoint に挿入することを許可します。</p></li>
</ol>
<blockquote>
<p>変更内容が有効になるまでに数時間かかる場合があることに注意してください。 <a href="/office365/admin/manage/manage-deployment-of-add-ins>Learn more</a>.</p>
</blockquote></td>
</tr>
</tbody>
</table>


## <a name="security--compliance"></a>[セキュリティとコンプライアンス](#tab/security)

このセクションは、コンテンツのセキュリティとデータ使用について満たす必要がある法律、規制、技術の標準が業務にある場合に利用します。

**Microsoft Forms のデータはどこに保存されていますか?**

Microsoft Forms のデータは、米国内およびヨーロッパに配置されているサーバーに保存されます。 すべてのデータが米国内にありますが、2017 年 5 月以降に Microsoft Forms の使用を開始したヨーロッパを拠点とするテナントのデータは除きます。 それらのデータはヨーロッパのデータベースに保存されます。

**Microsoft Forms は準拠していますか?**

2018 年 5 月現在、Microsoft Forms は GDPR のコンプライアンス要件を満たしています。 詳細については、[GDPR に対応した Microsoft 365 データ主体の要求](/microsoft-365/compliance/gdpr-dsr-office365?toc=/microsoft-365/enterprise/toc.json)に関するページを参照してください。

**FERPA と BAA の保護が整っていますか?**

Microsoft Forms は、[FERPA](https://www.microsoft.com/trustcenter/compliance/ferpa) と [BAA の保護基準](https://www.microsoft.com/TrustCenter/Compliance/HIPAA)を満たしています。

*ユーザーが組織を離れた後でも、ユーザー アカウントに保存されるユーザー数とデータ量に制限はありますか?*

現時点では、アカウントのプロビジョニングが組織のオンライン サービス契約の範囲内にある限り、データが保持されるユーザー数に制限はありません。 また、ユーザー アカウントに保存されるデータ量に制限はありません。

*フォームの元の所有者は組織に所属していないか、Microsoft Forms ライセンスが削除されています。作成したフォームに関連付けられているデータはどうなりますか?*

アカウント関連のデータはすべて、テナント (Azure AD) からユーザー アカウントが削除されてから 30 日後に削除されます。

## <a name="faq"></a>FAQ

**Microsoft フォームは何に使用できますか?**

Microsoft Forms は、アンケート、クイズ、投票を簡単に作成できる、シンプルな軽量アプリです。 教育機関では、テストの作成、教師と親からのフィードバックの収集、クラスや教職員の活動計画に使用できます。 ビジネス組織では、お客様からのフィードバックの収集、従業員の満足度の測定、製品や業務の改善、会社のイベントの計画に使用できます。

**Microsoft Forms を利用できるのは誰ですか?**

Microsoft アカウント (Hotmail、Live、Outlook.com) をお持ちであれば、誰でも Microsoft Forms を無料でご利用いただけます。 Office 365 Education および Microsoft 365 Apps for business の次のお客様は、Microsoft フォームも使用できます。

Office 365 Education

  - Office 365 A1 Plus

  - Office 365 A5

  - 退職前に E3 Office 365 Educationを購入した既存のお客様

Microsoft 365 Apps for business

  - Microsoft 365 Business Basic

  - Microsoft 365 Business Standard

  - Microsoft 365 Business Premium

  - Microsoft 365 Apps for enterprise

  - Microsoft 365 Enterprise E1、E3、および E5 プラン

  - Office 365 Enterprise E4 をサポート終了前に購入したお客様

[forms.office.com](https://forms.office.com/) にログインして、アンケート、クイズ、投票の作成を開始します。

**Microsoft 365 アカウントがないユーザーも Microsoft Forms でアンケートやテストを送信できますか?**

Microsoft Forms の作成者は、組織外のユーザーがアンケートやテストに回答できるようにするため、設定を切り替えることができます。 この場合、ユーザーは匿名で回答を送信することになります。 アンケートやテストに記入したユーザーを知りたい場合は、アンケーの一環として回答者に名前の記入を求めることができます。

**作成できるフォームの数と、フォームが受け取ることのできる回答の数に制限はありますか?**

Office 365 Education および Microsoft 365 Apps for business のお客様は、最大 200 個のフォームを作成でき、各フォームは最大 50,000 件の回答を受け取ることができます。 Microsoft アカウント (Hotmail、Live、または Outlook.com) を持つ Microsoft Forms ユーザーは、最大 200 個のフォームを作成できます。各フォームは、有料アカウントの場合は最大 1,000 件、無料アカウントの場合は最大 200 件の回答を受け取ることができます。 [Forms でのフォーム、質問、回答、文字数の制限](https://support.microsoft.com/office/form-question-response-and-character-limits-in-microsoft-forms-ec15323d-92a4-4c33-bf88-3fdb9e5b5fea)の詳細情報をご覧ください。

さらに多くの回答が必要な場合は、既存の回答を Excel ブックにエクスポートした後、アンケートやテストからこれらの回答をクリアすることをお勧めします。 これにより、一度クリアされたその他の回答を収集します。

**Microsoft Forms はどの Web ブラウザーで動作しますか?**

Microsoft Forms は、Internet Explorer 11 以上、Edge、Chrome (最新バージョン)、Firefox (最新バージョン)、Android 上の Chrome (最新バージョン)、iOS 上の Safari (最新バージョン) に最適化されています。

**Microsoft Forms はどの言語で使用できますか?**

Microsoft Forms の[サポートされる言語](https://support.microsoft.com/office/languages-supported-by-microsoft-forms-c17498cb-cbf6-4178-ae83-bd24934398ac)と[言語の設定](https://support.microsoft.com/office/language-settings-for-microsoft-forms-b282f9aa-0fe4-4290-b1e1-827a8a35ac27)を参照してください。

**Microsoft Forms は Microsoft InfoPath を置き換えるアプリケーションですか?**

いいえ。 Microsoft InfoPath は、ワークフローの自動化を有効にできるカスタマイズ可能なフォームを作成するためのソリューションでしたが、Microsoft Forms はアンケートとテストを通じて情報をすばやく収集するための軽量の基本アプリです。

Microsoft InfoPath は、SharePoint リスト、フロー、および PowerApps で置き換えられています。これらは従来の会社のフォームのデジタル化、ワークフローの自動化、およびビジネス プロセスの変換のための最新のソリューションです。 [詳細情報](https://products.office.com/business/business-process-automation) を参照してください。

**製品のバグや機能リクエストなどのフィードバックはどこから送信できますか?**

ご意見をお聞かせください。\! Microsoft Forms に関するフィードバックを送信するには、フォームの右上隅に移動して **[その他のフォームの設定]** ![[その他のオプション ボタン]](./media/image2.png) \> **[フィードバック]** の順に選択します。

>[!Note]
>詳細については、「[Microsoft Forms についてよく寄せられる質問](https://support.microsoft.com/office/frequently-asked-questions-about-microsoft-forms-495c4242-6102-40a0-add8-df05ed6af61c)」を参照してください。

