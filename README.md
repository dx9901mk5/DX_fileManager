# DX檔案管理器 (DX File Manager)

> [!IMPORTANT]
> **發布通道公告 / Release Channel Notice**
> - **DX檔案管理器 主程式已全面移至 Google Play 商店發行**，本 GitHub 儲存庫**已移除所有主程式 APK 並停止於 GitHub 更新主程式**。
> - 本倉庫 Releases **僅維持提供專屬外掛「DX輔助助手 (`DX_Helper`)」**。
>
> ---
> - **The main DX File Manager app is now distributed exclusively via Google Play.** All main-app APKs have been removed from GitHub Releases and will no longer be updated here.
> - GitHub Releases **now hosts ONLY the companion plugin `DX_Helper`**.

一個專為 Android 設計的高效率多視窗／多面板檔案管理器，結合本機檔案管理、雲端與網路掛載（Google Drive、OneDrive、SMB、SFTP、FTP、WebDAV）、自由小視窗拖曳桌面捷徑、AI 檔案整理助理與四國語言即時切換。

---

## 參加 Google Play 封閉測試（三步驟）/ Join Google Play Closed Testing (3 Steps)

目前 Google Play 版處於封閉測試階段，請依序完成以下三個步驟即可從 Google Play 商店下載體驗：

1. **步驟 1｜加入測試人員 Google 群組**  
   👉 [https://groups.google.com/g/dx-file-manager-testers](https://groups.google.com/g/dx-file-manager-testers)  
   （群組信箱：`dx-file-manager-testers@googlegroups.com`，請使用與手機 Play 商店相同的 Google 帳號點擊「加入群組」）
2. **步驟 2｜成為測試人員（網頁確認加入）**  
   👉 [https://play.google.com/apps/testing/com.dx9901mk5.filemanager](https://play.google.com/apps/testing/com.dx9901mk5.filemanager)  
   （點擊頁面中的「成為測試人員」按鈕）
3. **步驟 3｜前往 Google Play 商店下載安裝**  
   👉 [https://play.google.com/store/apps/details?id=com.dx9901mk5.filemanager](https://play.google.com/store/apps/details?id=com.dx9901mk5.filemanager)

---

1. **Step 1 | Join the Tester Google Group**  
   👉 [https://groups.google.com/g/dx-file-manager-testers](https://groups.google.com/g/dx-file-manager-testers) (`dx-file-manager-testers@googlegroups.com`)
2. **Step 2 | Opt-in on the Web**  
   👉 [https://play.google.com/apps/testing/com.dx9901mk5.filemanager](https://play.google.com/apps/testing/com.dx9901mk5.filemanager)
3. **Step 3 | Install from Google Play (Android)**  
   👉 [https://play.google.com/store/apps/details?id=com.dx9901mk5.filemanager](https://play.google.com/store/apps/details?id=com.dx9901mk5.filemanager)

---

## DX輔助助手 (`DX_Helper`) 用途說明與下載

### 為什麼需要 `DX_Helper`？
受限於 Google Play 商店政策規範，Play 版主程式不請求 `REQUEST_INSTALL_PACKAGES`（安裝未知應用）與 `QUERY_ALL_PACKAGES`（查詢所有已安裝套件）等敏感權限。因此我們將進階系統功能抽離為同簽名專屬外掛 **`DX_Helper`**，由 GitHub 獨立提供，**完全不影響 Play 版合規性**。

### 安裝 `DX_Helper` 後可解鎖的功能
安裝 **`DX_Helper`** 並搭配 **Google Play 版 DX檔案管理器** 後，主程式會自動偵測此外掛並開放以下功能：
1. **讀寫 `Android/data` 與 `Android/obb` 受限系統目錄**：
   - 未安裝外掛時 Play 版側邊欄會自動隱藏系統受限入口；安裝 `DX_Helper` 並授權 Shizuku 後，側邊欄即自動顯示 **`Android/data`** 與 **`Android/obb`** 快速入口，支援完整瀏覽、複製、搬移與刪除操作。
2. **透過 Shizuku 靜默批次安裝 APK**：
   - 在 Play 版長壓或選取 `.apk` 檔案時，功能選單會自動出現 **「用 DX Shizuku 靜默安裝」**，免去系統安裝器反覆確認。
3. **已安裝應用程式列表與備份轉發分享**：
   - Play 版側邊欄會自動開放 **「應用程式」** 專區，瀏覽裝置所有已安裝 App 並匯出備份 APK / Split APKs (`.apks`)。
   - `DX_Helper` 本身亦內建 **「應用程式備份與轉發分享」** 介面，可直接搜尋、多選 App 打包後透過系統分享選單選擇 **DX檔案管理器** 儲存至指定資料夾。
4. **外掛自我更新**：
   - `DX_Helper` 內建「檢查外掛更新 (GitHub)」按鈕，可自動檢查並更新至最新外掛版本。

### 下載 DX輔助助手 / Download `DX_Helper`
前往 [GitHub Releases](https://github.com/dx9901mk5/DX_fileManager/releases/latest) 下載：
- **`DX_Helper-v<version>-release.apk`**（固定簽名，可直接覆蓋更新）

---

## Why `DX_Helper`? (English Summary)
To keep the Google Play main app 100% compliant (without `REQUEST_INSTALL_PACKAGES` or `QUERY_ALL_PACKAGES`), advanced system capabilities are provided through this same-signature companion plugin **`DX_Helper`**:
- **Access `Android/data` & `Android/obb`**: Automatically reveals `Android/data` and `Android/obb` shortcuts in the Play edition sidebar once `DX_Helper` + Shizuku are active.
- **Silent APK Installation via Shizuku**: Enables batch silent APK installation directly from the Play edition context menu.
- **Installed Apps List & APK Backup/Share**: Unlocks the "Apps" category in the Play edition and includes a standalone **"App Backup & Share"** UI inside `DX_Helper` (supports Split APKs `.apks` and sharing directly into DX File Manager to save to any folder).
- Download **`DX_Helper-v<version>-release.apk`** from [GitHub Releases](https://github.com/dx9901mk5/DX_fileManager/releases/latest).

---

## 開發者 / Developer
- **dx9901mk5** — [GitHub Repository](https://github.com/dx9901mk5/DX_fileManager)
