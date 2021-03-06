---

copyright:

  years: 1994, 2018

lastupdated: "2018-05-22"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}


# 將使用者新增至 SoftLayer 帳戶
{: #customerportal_addusertocpacct}

一位以上的使用者可以與帳戶的相關聯產品及服務互動。如果您是主要使用者，則隨時都可以新增使用者。
{:shortdesc}

如果您要管理 {{site.data.keyword.BluSoftlayer_full}} 基礎架構使用者，則可管理的 SoftLayer 帳戶取決於指派給使用者帳戶的存取權。您可以管理的帳戶也取決於帳戶的設定方式。如果您是主要使用者，或身為帳戶擁有者而具有管理存取權，則可以管理其他客戶入口網站使用者。如果您的帳戶未設定成主要使用者，則可以管理使用者設定檔。

根據您的存取權，您可以從「使用者」視窗管理 SoftLayer 帳戶或是其他使用者的帳戶。[客戶入口網站 ![外部鏈結圖示](../icons/launch-glyph.svg)](https://control.softlayer.com/){:new_window} 中的「使用者」視窗會顯示與帳戶相關聯的使用者。「使用者」視窗上可用的互動會根據唯一的帳戶權限集而不同。
  * 如果您是帳戶的主要使用者，則可以看到與帳戶相關聯的所有使用者。

  如果您必須共用帳戶的主要登入認證，共用認證時請務必謹慎。您的主要登入控制了帳戶的每個層面；請小心保護。若要讓其他使用者使用客戶入口網站，您可以設定個別使用者，或以許可權為基礎的使用者。建立以許可權為基礎的使用者，可確保您可以最大限度地控制哪些人可以與帳戶的特定層面進行互動。
  {:tip}

  * 如果您具有管理存取權，則可以看到您新增的所有使用者。如果您已將管理其他使用者的許可權提供給那些使用者，則也可以看到他們新增的任何使用者。您也可以管理與帳戶相關聯的任何使用者，包括編輯客戶入口網站的存取權、變更使用者狀態，以及移除使用者。
  * 如果您不是帳戶的主要使用者，而且沒有管理存取權，則只會顯示您的設定檔。您可以與自己的帳戶互動（包括檢視 API 金鑰、編輯 VPN 存取權，以及新增外部鑑別）。

若要從 {{site.data.keyword.Bluemix_notm}} 主控台管理使用者，請參閱[帳戶設定](/docs/account/adminpublic.html#signing-up-for-ibm-cloud)小節，及[管理身分及存取](/docs/iam/quickstart.html#getstarted)。如需 {{site.data.keyword.Bluemix_notm}} 主控台的相關資訊，請參閱 [{{site.data.keyword.Bluemix_notm}} 主控台的運作方式](/docs/overview/ui.html#ui)。

組織內的不同人員有不同的角色及責任，而且使用者許可權集不是一體適用。因此，您可以將具有角色的使用者新增至客戶入口網站，以提供恰好只針對其特定角色所需的存取權。如果錯誤或未授權地進行變更，則可以追蹤回到使用者或群組。因此，您可以提供適當的訓練或更新使用者許可權，讓風險降到最低。您的使用者便可以專注於客戶入口網站內的指定角色。

請使用下列步驟，以將使用者新增至帳戶。

1. 使用唯一的認證來存取客戶入口網站。
2. 從導覽列中，選取**帳戶 > 使用者**。
3. 按一下**新增使用者**。
4. 完成**個人資訊**區段中的必要欄位。提供狀態、使用者名稱，以及客戶入口網站通訊及通知（包括設定帳戶密碼的起始通知）用的電子郵件位址。

  您可以選擇按一下**使用預設公司資訊**勾選框來移入公司地址，而不是輸入使用者的地址。
  {: tip}

5. 完成**登入設定**區段中的必要欄位。指定使用者是否可以編輯設定、是否限制 IP 位址，以及使用者是否需要設定及使用安全問題。而且，針對任何未使用 IBM ID 的使用者，您可以設定密碼在多久以後到期。
**附註：**
* 如果您使用 IBM ID 進行鑑別，則請遵循**登入**下的指示，以在 [IBM ID 設定檔 ![外部鏈結圖示](../icons/launch-glyph.svg)](https://www.ibm.com/account/profile){:new_window} 中更新密碼。
* 按一下**將入口網站密碼用於 VPN** 勾選框，以同步化客戶入口網站及 VPN 密碼。
6. 按一下**新增使用者**。

在您建立使用者的帳戶之後，使用者會收到完成設定其帳戶的電子郵件通知。使用者必須設定密碼，以及選擇性地建立安全問題（如果您指出它們是必要項目）。

沒有主要使用者管理存取權的使用者登入客戶入口網站的方式，取決於已在其 SoftLayer 帳戶中提供使用者存取權的主要使用者：
  * 如果主要使用者具有 IBM ID 進行鑑別，則主要使用者所建立的每一位使用者都會有 IBM ID。
  * 如果主要使用者具有「{{site.data.keyword.BluSoftlayer_notm}} 基礎架構 ID」進行鑑別，則主要使用者所建立的每一位使用者都會有「{{site.data.keyword.BluSoftlayer_notm}} 基礎架構」使用者名稱。主要使用者以及主要使用者所建立的每一位使用者都必須執行移轉工具，才能切換至 IBM ID。
  * 如果不是上述這些情況，例如，如果是 IBM 事業夥伴，則請聯絡「支援中心」來判定要使用的使用者 ID。

## 設定帳戶上的使用者許可權
{: #cp_setuserpermsacct}

請使用下列步驟，以設定您剛才新增的使用者的許可權。

1. 按一下**許可權**圖示，其以帶鎖的使用者圖例表示。
2. 更新新增使用者的所有標籤上的**使用者許可權**。
> **附註：**從**快速許可權**清單中選取選項，以檢視三種使用者類型的許可權集。按一下**設定許可權**以選取許可權集，或選取每一個可用標籤上的個別選項來自訂使用者的可存取性。
3. 按一下**新增入口網站許可權**以新增許可權，或按一下**重設許可權**以重設使用者的許可權。
4. 按一下**裝置存取權**圖示（以三部伺服器表示）。
5. 按一下您要讓使用者能夠存取的每一個裝置的裝置勾選框。
6. 在選取裝置之後，請按一下**更新裝置存取權**。

您會收到一封電子郵件，其中所含的鏈結及資訊可以引導您完成設定  IBM ID 以鑑別此帳戶。如果帳戶要使用 IBM ID 進行鑑別，則這些步驟可能包括建立新的 IBM ID。邀請會在 7 天後到期，但您可以聯絡管理者重新傳送邀請。

在所有其他鑑別情況下，於新增使用者之後，使用者便隨時可以登入客戶入口網站。之後，使用者便可以使用與帳戶相關聯的各種產品和服務。您隨時可以停用使用者。
