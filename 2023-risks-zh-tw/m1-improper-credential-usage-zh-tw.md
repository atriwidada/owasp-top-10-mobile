---

layout: col-sidebar
title: "M1: 不當的憑證使用"
---

# 威脅主體

**應用層面 特定**

在手機應用程式中，利用硬編碼的憑證和不當的憑證使用的威脅主體，包含使用公開或自製的工具來進行的自動化攻擊。這樣的威脅主體有可能找到並利用硬編碼的憑證，或能利用因憑證使用不當從而產生的弱點。

# 攻擊媒介

**利用難度 簡單**

攻擊者可以利用硬編碼的憑證和憑證使用不當的漏洞。一旦這些漏洞被識別出來，攻擊者可以使用硬編碼的憑證來未經授權地訪問手機應用程式的敏感功能。他們還可以濫用憑證，例如通過使用未經正確驗證或存儲的憑證來獲取訪問權限，從而繞過合法訪問的必要。

# 安全層面的強度

**普及性 常見**

**偵測性 簡單**

對憑證管理執行不當，例如使用硬編碼的憑證和不當的處理，可能導致嚴重的安全弱點。全面的安全測試流程目的應該為識別這些問題。例如，安全測試人員應該嘗試在手機應用程式的原始碼或配置文件中識別硬編碼的憑證。

# 技術性影響

**影響程度 嚴重**

憑證管理不當可能導致多個重大的技術影響。未經授權的使用者可能會進入手機應用程式或其後端系統中的敏感信息或功能。這可能引起數據洩漏、用戶隱私損失、欺詐活動，以及潛在訪問管理功能。

# 業務影響

**影響程度 嚴重**

憑證管理不善，包括硬編碼的憑證和不當的憑證使用，對於企業可能產生重大影響：

* 名聲損害
* 資訊竊盜
* 詐欺
* 未經授權的訪問資料

# 我是否容易受到「不當的憑證使用」的攻擊？

當手機應用程式使用硬編碼的憑證或憑證被不當使用時，可能產生不安全的憑證管理。以下是您的手機應用程式可能容易受到攻擊的一些指標：

* **硬編碼的憑證** - 如果手機應用程式在應用程式原始碼或任何配置文件中包含硬編碼的憑證，這是一個明確的漏洞指標。
* **不安全的憑證傳輸** - 如果憑證在未加密或通過不安全的通道傳輸，這可能表明存在漏洞。
* **不安全的憑證存儲** - 如果手機應用程式以不安全的方式在設備上存儲使用者憑證，這可能代表存在漏洞。
* **脆弱的用戶身份驗證** - 如果用戶身份驗證依賴於脆弱的協定或容易被規避，這可能是漏洞的跡象。

如果您注意到以上任何一點，您的手機應用程式可能存在潛在的安全風險，建議採取相應的措施以加強憑證管理和提高安全性。

# 如何防止「不當的憑證使用」？

避免不安全的憑證管理包括不使用硬編碼的憑證並正確處理使用者憑證。

**避免使用硬編碼的憑證**

硬編碼的憑證容易被攻擊者發現，為未經授權的使用者提供了容易進入的途徑。請務必避免在手機應用程式的程式碼或配置文件中使用硬編碼的憑證。

**正確處理使用者憑證**

使用者憑證應總是以安全的方式存儲、傳輸和進行驗證：

* 在傳輸過程中加密憑證。
* 不要在設備上存儲使用者憑證。相反的，考慮使用安全的、可撤銷的訪問令牌。
* 實施強固的使用者身份驗證協議。
* 定期更新並更換使用的 API 金鑰或令牌

# 攻擊情境舉例

以下情境展示了在手機應用程式中的不當憑證使用：

**情境1:** 硬編碼的憑證：攻擊者發現手機應用程式原始碼中的硬編碼的憑證。他們使用這些憑證未經授權地訪問應用程式或後端系統中的敏感功能。

**情境2:** 不安全的憑證傳輸：攻擊者攔截手機應用程式和後端系統之間不安全傳輸的憑證。他們使用這些攔截到的憑證冒充合法用戶，未經授權地訪問資源。

**情境3:** 不安全的憑證存儲：攻擊者物理訪問用戶設備並從手機應用程式中提取存儲的憑證。攻擊者使用這些憑證未經授權地訪問用戶帳戶。

# 參考資料

- OWASP
    - [OWASP](https://www.owasp.org/index.php/OWASP_Top_Ten)
- External
    - [外部來源](http://cwe.mitre.org/)