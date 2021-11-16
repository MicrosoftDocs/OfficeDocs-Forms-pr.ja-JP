---
title: Microsoft Forms の管理者設定
ms.author: jokay
author: dumptruckjon
manager: kathyl
audience: Admin
ms.topic: how-to
ms.service: forms-pro
ms.localizationpriority: high
description: この記事では、Microsoft 365 管理者のための Microsoft Forms 設定について説明します。
ms.openlocfilehash: 371d3700a1d6157b3c65bc1b1b0224ef73f788a3
ms.sourcegitcommit: 09bdc82ce67e74495b6c58d9c842e31c17956fc3
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/12/2021
ms.locfileid: "60951551"
---
# <a name="administrator-settings-for-microsoft-forms"></a>Microsoft Forms の管理者設定

> [!Note]
> 管理者設定は、Office 365 Education および Microsoft 365 Apps for business でのみ使用できます。 これらの設定にアクセスするには、職場または学校のアカウントで [https://admin.microsoft.com](https://admin.microsoft.com/) にサインインします。

## <a name="microsoft-365-admin-center"></a>Microsoft 365 管理センター

Microsoft 365 管理センターでは、管理者は外部共有設定を制御したり、組織内のユーザーの名前を記録したり、内部フォームをフィッシングから保護したりできます。

これらの設定にアクセスする方法は次のとおりです。

1.  職場または学校のアカウントを使用して、[https://admin.microsoft.com](https://admin.microsoft.com/) にサインインします。

2.  **設定** \> **組織の設定** の順に選択します。

    >[!Note]
    > **設定** オプションが表示されない場合、左側のウィンドウで ![その他のオプション ボタン](./media/image2.png) **すべて表示** の順に選択します。
 
3.  **設定** ページの **サービス** タブで、**Microsoft Forms** をクリックします。

特定の設定については、下記の手順に従ってください。

### <a name="external-sharing"></a>外部共有

外部ユーザーがフォームまたはテストで組織内のユーザーとの共同作業を許可するかどうかを制御できます。 たとえば、組織内のユーザーがフォームを作成し、次のことを手伝ってもらいたい場合があるとします。

  - 組織外のユーザーにフォームへのリンクを送信し、外部のユーザーからの回答を収集します。

  - 組織外のユーザーとフォームで共同作業 (質問の編集、テーマのデザインの変更など) を行います。

  - 組織外のユーザーが独自の目的でフォームを複製できるように、フォームをテンプレートとして共有します。

  - フォームの結果の概要を組織外のユーザーと共有します。

>[!Tip]
>[共同作業するフォームの共有](https://support.microsoft.com/office/share-a-form-or-quiz-to-collaborate-d5bb5cf0-8401-4c15-bb8c-8e108cd7e69b) について説明します。

Microsoft 365 管理センターで外部共有設定を制御するには:

1.  **Microsoft Forms** ウィンドウでは、**外部共有** 設定には 4 つのオプションがあり、これらはすべて既定でオンになっています。 不要なオプションをオフにします。

    :::image type="content" source="./media/admin-settings-external-sharing.png" alt-text="外部共有のための Microsoft Forms 管理者設定":::

     >[!Note]
     >組織内のユーザーに[Outlook で投票を作成する](https://support.microsoft.com/office/create-a-poll-in-outlook-46893563-ab12-4bd0-aff7-26f5a488fea0) 機能を提供する場合、**フォームへリンクを送信して回答を収集する** のオプションを確実にオンにする必要があります。

2.  **[変更の保存]** を選択します。

### <a name="record-names-of-people-in-your-org"></a>組織内のユーザーの名前を記録する

フォーム レスポンダーの名前をキャプチャするかどうかを選択できます。

1.  **Microsoft Forms** ウィンドウでは、**組織内のユーザーの名の記録** の設定下にある**既定で名前の記録をする** の設定が既定でオンになっています。 応答時に名前を記録しない場合は、このオプションをオフにしてください。

    :::image type="content" source="./media/admin-settings-record-names.png" alt-text="名前の記録のための Microsoft Forms 管理者設定":::

1.  **[変更の保存]** を選択します。

### <a name="phishing-protection"></a>フィッシング対策

組織内のフォームの自動スキャンを設定して、フィッシングの検出を行うことができます。

1.  **[Microsoft Forms]** ウィンドウで、**[フィッシング保護]** の **[内部フィッシング保護]** 設定が既定でオンになっています。 組織内でフォームのフィッシング スキャンを行わない場合は、このオプションをオフにします。

    :::image type="content" source="./media/admin-settings-phishing.png" alt-text="フィッシング対策のための Microsoft Forms 管理者設定":::

2.  **[変更の保存]** を選択します。

### <a name="allow-youtube-and-bing"></a>YouTube と Bing を許可する

組織内のユーザーが Bing または YouTube ビデオの画像をアンケートに追加することを許可するかどうかを選択できます。

1.  **Microsoft Forms** ウィンドウでは、**YouTube と Bing を許可する**の下の**Bing search、YouTube 動画を含む** の設定が既定でオンになっています。 組織内のユーザーが YouTube.com からの動画や Bing.com からの画像をフォームに追加しないようにする場合は、このオプションをオフにします。

    :::image type="content" source="./media/admin-settings-youtube-bing.png" alt-text="YouTube と Bing のための Microsoft Forms 管理者設定":::

2.  **[変更の保存]** を選択します。

### <a name="turn-off-or-turn-on-microsoft-forms-user-license-assignment"></a>Microsoft Forms ユーザー ライセンスの割り当てを有効または無効にする

ユーザーのMicrosoft Formsをオフにすると、そのユーザーはMicrosoft Forms を使用できません。 **Forms** タイルは、Microsoft 365 アプリ起動ツールとホームページで非表示になります。 個人のMicrosoft Forms で有効または無効にするステップについては[Microsoft 365 Apps for business のユーザーにライセンスを割り当てる](https://support.microsoft.com/topic/997596b5-4173-4627-b915-36abac6786dc) を確認してください。

組織全体で[Microsoft Formsを有効または無効にする](turn-off-turn-on-microsoft-forms.md)かを選択することもできます。
