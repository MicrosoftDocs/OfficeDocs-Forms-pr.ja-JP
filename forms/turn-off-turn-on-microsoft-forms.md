---
title: Microsoft Forms を有効または無効にする
ms.author: jokay
author: dumptruckjon
manager: kathyl
audience: Admin
ms.topic: how-to
ms.service: forms-pro
ms.localizationpriority: high
description: この記事では、Microsoft 365管理者が組織全体または組織内の特定のユーザーのMicrosoft Formsを有効または無効にする方法について説明します。
ms.openlocfilehash: 2d1280bd7d61dc8b31cfb84dfeaced2662603e4f
ms.sourcegitcommit: 09bdc82ce67e74495b6c58d9c842e31c17956fc3
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/12/2021
ms.locfileid: "60951527"
---
# <a name="turn-off-or-turn-on-microsoft-forms"></a>Microsoft Forms を有効または無効にする

既定では、組織内のすべてのユーザーに対して[ Microsoft Forms](https://support.microsoft.com/office/what-is-microsoft-forms-6b391205-523c-45d2-b53a-fc10b22017c8) が有効になっています。 [管理者](https://support.microsoft.com/topic/eac4d046-1afd-4f1a-85fc-8219c79e1504) の場合は、[Microsoft Formsの設定](https://support.microsoft.com/office/set-up-microsoft-forms-cc52287a-4550-464d-9a1b-457bf9df2240)をオフにするか、組織全体または特定のユーザーに対してもう一度オンにすることができます。

## <a name="turn-off-microsoft-forms-for-everyone-in-your-organization"></a>組織内のすべてのユーザーのMicrosoft Formsをオフにする

1.  [Microsoft Azure](https://portal.azure.com/)にログインします。

2.  左ペインで **Azure Active Directory** をクリックします。

3.  **エンタープライズ アプリケーション**をクリックします。

4.  必要なサービスに移動し、**アプリケーションの種類**\>と**CollabDBService** および **Microsoft Applications**\>と**Microsoft Forms**の両方について手順 5 - 7 を繰り返します。
    
      - **アプリケーションの種類** ドロップダウン リストの下の検索フィールドに、**CollabDBService**と入力してください。 検索結果の一覧で**CollabDBService**を選択します。
    
      - **アプリケーションの種類** ドロップダウン リストで、**Microsoft Applications**を選択します。 **アプリケーションの種類** ドロップダウン リストの下の検索フィールドに**Microsoft Forms**と入力し、検索結果一覧で **Microsoft Forms** を選択します。

5.  **管理**で **プロパティ**をクリックします。

6.  このオプション**ユーザーのサインインを許可しますか?** で、**いいえ**を選択します。

7.  [**保存**] をクリックします。

## <a name="turn-off-microsoft-forms-for-specific-people-in-your-organization"></a>組織内の特定のユーザーのMicrosoft Formsを無効にする

1.  職場や学校のアカウントを使って、グローバル管理者として Office 365 にサインインします。[サインインの手順を参照](https://support.microsoft.com/office/where-to-sign-into-microsoft-365-for-business-e9eb7d51-5430-4929-91ab-6157c5a050b4)。

2.  Microsoft 365 管理センターで、**ユーザー** \> **アクティブなユーザー**の順にクリックします。

3.  Microsoft Formsを無効にしたいユーザーの名前の横にあるボックスを選択します。

4.  リボンで、**製品のライセンスを管理**をクリックします。

5.  表示されたアカウント フォームの **ライセンスとアプリ** タブで、 アプリのセクションを展開し、Microsoft Forms オプションまでスクロールします。 

    :::image type="content" source="./media/turn-forms-off-on-licenses-apps.jpg" alt-text="Microsoft 365 管理センターのアカウント オプション フォーム":::

6.  チェック ボックスをオフにし、Microsoft Formsを無効にします。 有効にするには、チェック ボックスをオンにします。

    :::image type="content" source="./media/turn-forms-off-on-plan-e1.jpg" alt-text=" Microsoft Forms の切り替え":::

     > [!Note]
     > [この一覧を確認](https://support.microsoft.com/office/office-licenses-that-include-microsoft-forms-efa14679-5d99-47c5-bdf1-2fc838767f7e)し、Microsoft Formsを含む Office ライセンスがあるかどうかを確認します。 ライセンスが表示されている場合は、Microsoft Forms のチェック ボックスをオフにして、ユーザー アクセスを完全に無効にする必要があります。

7.  **アプリ**の一覧の下部にある**変更の保存**をクリックします。

## <a name="i-turned-on-microsoft-forms-but-people-in-my-organization-still-cant-access-it"></a>Microsoft Formsを有効にしたが、組織内のユーザーがまだアクセスできない

Microsoft Formsが有効になっていることを確認するには、Microsoft Azureで次の設定を確認します。

1.  [Microsoft Azure](https://portal.azure.com/)にログインします。

2.  左ペインで **Azure Active Directory** をクリックします。

3.  **エンタープライズ アプリケーション**をクリックします。

4.  必要なサービスに移動し、**アプリケーションの種類**\>と**CollabDBService** および **Microsoft Applications**\>と**Microsoft Forms**の両方について手順 5 - 7 を繰り返します。
    
      - **アプリケーションの種類 **ドロップダウン リストの下の検索フィールドに、**CollabDBService**と入力します。 検索結果の一覧で**CollabDBService**を選択します。
    
      - **アプリケーションの種類** ドロップダウン リストで、**Microsoft Applications**を選択します。 **アプリケーションの種類** ドロップダウン リストの下の検索フィールドに**Microsoft Forms**と入力し、検索結果一覧で **Microsoft Forms** を選択します。

5.  **管理**で **プロパティ**をクリックします。

6.  このオプションの、**ユーザーがサインインできるようにしますか?** で、**はい** を選択します。

7.  [**保存**] をクリックします。

    >[!Note]
    >組織内のユーザーがMicrosoft Formsにアクセスできるように、SharePoint サービスも有効にする必要があります。

## <a name="feedback-for-microsoft-forms"></a>Microsoft Forms のフィードバック

ご意見をお聞かせください。\! Microsoft Forms に関するフィードバックを送信するには、フォームの右上隅に移動して **その他のフォームの設定** ![その他のオプション ボタン](./media/image2.png)\> **フィードバック** の順にクリックします。

