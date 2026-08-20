<div align="center">
  <img width="90" height="90" src="/iisend.svg" alt="iisend logo">

  # iisend

  Windows / macOS / Linux 上的 iOS 側載助手
</div>

---

## 這是什麼

`iisend` 是一個 iOS 側載工具，用來把 App 安裝到自己的 iPhone / iPad 上，
不需要越獄，只要一組 Apple ID。

主要功能：

- 一鍵安裝 **iiTwins**（自訂的 LiveContainer + SideStore 版本）
- 匯入任何 `.ipa` 檔案安裝到裝置
- 自動處理配對檔（pairing file）與憑證
- 檢視 / 撤銷開發憑證與 App ID

## 系統需求

**Windows**：需要安裝 iTunes 以提供 `usbmuxd`（裝置連線服務）。

> ⚠️ **Microsoft Store 版的 iTunes 不含 Apple Mobile Device Service**，
> 會出現 `Failed to connect to usbmuxd: device socket io failed`。
> 請安裝 Apple 官網的桌面版 iTunes，或單獨安裝 `AppleMobileDeviceSupport64.msi`。

## 授權與來源

本專案是 [nab138/iloader](https://github.com/nab138/iloader) 的衍生作品。

- 原始程式碼採用 **MIT License**，版權歸原作者 nab138 所有（見 [LICENSE](LICENSE)）。
- 本專案的名稱與圖示為獨立設計，**未使用**原專案的品牌素材。
- 本專案為**非官方**的個人修改版本，與原作者無任何關聯，
  也未獲得原作者的背書或贊助。

原專案相關連結：

- 官方網站：<https://iloader.app>
- 原始碼：<https://github.com/nab138/iloader>

## 與原專案的差異

| 項目 | 變更 |
|---|---|
| 安裝來源 | 指向自訂的 iiTwins 版本 |
| 安裝選項 | 移除官方 SideStore / LiveContainer 的四個安裝按鈕 |
| 識別碼 | `com.tyu.iisend`（與原專案並存，不衝突） |
| 憑證儲存 | 使用獨立的 keyring 空間 |
| 自動更新 | 指向本專案的 releases |
