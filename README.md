# DX檔案管理器 (DX File Manager)

> [!IMPORTANT]
> **發布通道轉移公告 / Release Channel Notice**
> - **Google Play 正式版通過審核後，本 GitHub 儲存庫 Releases 將僅保留「DX Shizuku 輔助安裝器 (`DX_Helper`)」**，主程式將統一移至 Google Play 商店發行，並於本頁面放上正式版 Google Play 商店連結（`https://play.google.com/store/apps/details?id=com.dx9901mk5.filemanager`，審核通過後正式啟用）。
> - 目前提供的 GitHub 版主程式 APK（`DX_fileManager-v*-full-release.apk`）為過渡預覽版本，**內建 16 天使用期限**。
>
> ---
> - **Once the Google Play release passes review, GitHub Releases will retain ONLY the "DX Shizuku Helper (`DX_Helper`)" plugin.** The main app will be distributed exclusively via Google Play, and the official Play Store link will be posted right here.
> - Current GitHub full-edition APKs (`DX_fileManager-v*-full-release.apk`) are transitional preview builds with a **built-in 16-day usage limit**.

一個專為 Android 設計的高效率多視窗／多面板檔案管理器，結合本機檔案管理、雲端與網路掛載、自由小視窗拖曳桌面捷徑、Shizuku 靜默安裝與 AI 檔案整理助理，並支援繁體中文、简体中文、English、日本語四國語言即時切換。

A high-efficiency multi-pane & freeform-window file manager for Android featuring local storage management, cloud/network mounts, drag-to-desktop shortcuts, Shizuku silent APK installation, AI file organization assistant, and instant 4-language UI switching (Traditional Chinese, Simplified Chinese, English, Japanese).

---

## 主要功能 / Key Features

- **多面板與自由小視窗操作 / Multi-Pane & Freeform Window**
  - 支援雙／三面板瀏覽、側邊欄快速導覽與自訂比例；可開啟多個 `WINDOWING_MODE_FREEFORM` 自由小視窗進行跨視窗與跨 App 拖曳。
  - Dual/three-pane browsing with customizable ratios, plus multiple `WINDOWING_MODE_FREEFORM` small windows for cross-window and cross-app drag-and-drop.
- **雙指／滑過多選與拖曳手勢 / Multi-Select & Drag Gestures**
  - 長壓 `0.75s` 進入多選，支援第二指點擊與滑過多選；手指停頓 `350ms` 後再移動即鎖定為純拖曳模式，避免誤選其他檔案。
  - Long-press (`0.75s`) to enter multi-select with second-finger tap and sweep-select; pausing for `350ms` and moving locks into pure drag mode.
- **任意檔案／資料夾桌面捷徑 / Drag-to-Desktop Shortcuts**
  - 拖曳任何檔案或資料夾出小視窗至桌面（或從功能表／底部操作列點擊「在桌面建立捷徑」），支援圖片／影片縮圖、APK 圖示與各類檔案專屬圖示，多選複合類別時自動批次建立。
  - Drag any file or folder out to the launcher desktop (or use the context menu / bottom bar action) to pin shortcuts with real thumbnails, APK icons, or type badges; multi-select supports batch shortcut creation.
- **雲端與網路掛載 / Cloud & Network Mounts**
  - 支援 Google Drive（OAuth 2.0）、OneDrive（PKCE）、SMB（SMBv2/v3 區網掃描、網域/訪客匿名登入、大檔串流與同掛載移動）、SFTP、FTP、WebDAV。
  - Built-in support for Google Drive (OAuth 2.0), OneDrive (PKCE), SMB (SMBv2/v3 LAN scan, Domain/Guest login, true streaming & server-side move), SFTP, FTP, and WebDAV.
- **AI 檔案整理助理 / AI File Assistant**
  - 支援 Gemini、DeepSeek、GPT (OpenAI)、Claude、Grok 與深度思考模式，協助分類、重命名與整理建議。
  - Integrates Gemini, DeepSeek, GPT (OpenAI), Claude, and Grok with optional thinking mode for smart organization.
- **Shizuku 靜默安裝與應用管理 / Shizuku Silent Install & App Manager**
  - 支援透過 Shizuku 靜默批次安裝 APK、已安裝應用檢視與備份匯出。
  - Batch silent APK installation via Shizuku, plus installed app inspection and APK backup export.
- **垃圾桶與加解密壓縮 / Recycle Bin, Crypto & Archives**
  - 內建 `.dx_trash` 30 天自動清理垃圾桶、ZIP/7Z/TAR 壓縮解壓縮與 `.dxe` AES-256 檔案加解密。
  - 30-day `.dx_trash` recycle bin, ZIP/7Z/TAR archive support, and `.dxe` AES-256 encryption/decryption.

---

## 下載與安裝 / Download & Install

- **Google Play 正式版**（審核通過後正式開放）：[Google Play Store](https://play.google.com/store/apps/details?id=com.dx9901mk5.filemanager)
- 前往 [GitHub Releases](https://github.com/dx9901mk5/DX_fileManager/releases/latest) 可下載（皆為固定簽名，可直接覆蓋更新；**Play 正式通過後 GitHub 僅保留第 2 項輔助安裝器**）：

1. **DX 檔案管理器 GitHub 過渡版（主程式，內建 16 天使用期限）**：`DX_fileManager-v<version>-full-release.apk`
   - Play 審核通過前之過渡完整版主程式，到期後請改用 Google Play 正式版。
2. **DX Shizuku 輔助安裝器（Play 正式通過後唯一保留於 GitHub 之外掛）**：`DX_Helper-v<version>-release.apk`
   - 本 App 為 **DX檔案管理器 專屬的 Shizuku 輔助用安裝器**，**同時支援 Google Play 版與 GitHub 版主程式**。
   - **支援 Google Play 版觸發能力**：安裝此輔助安裝器並授權 Shizuku 後，Google Play 版 DX檔案管理器 會自動偵測此外掛；當您在 Play 版內長壓任何 `.apk` 檔案時，功能選單會自動出現 **「用 DX Shizuku 靜默安裝」** 選項供選擇安裝 APK。
   - **外掛自我更新**：DX Shizuku 安裝助手內建「檢查外掛更新 (GitHub)」按鈕，可自動檢查 GitHub 最新外掛版本並下載安裝。

- **Official Google Play Edition** (available once Play review is approved): [Google Play Store](https://play.google.com/store/apps/details?id=com.dx9901mk5.filemanager)
- Download the signed APKs from [GitHub Releases](https://github.com/dx9901mk5/DX_fileManager/releases/latest) (**Once Google Play is approved, only `DX_Helper` will remain on GitHub**):
  - **`DX_fileManager-v<version>-full-release.apk`**: Transitional GitHub full edition (**16-day built-in usage limit**).
  - **`DX_Helper-v<version>-release.apk`**: Dedicated Shizuku helper installer plugin for **DX File Manager** (works with both the **Google Play edition** and the **GitHub edition**—when installed, the Play edition automatically detects the plugin and reveals the Shizuku APK install option in the context menu; includes built-in GitHub self-update check & download/install).

---

## 權限說明 / Permissions

- `MANAGE_EXTERNAL_STORAGE`（所有檔案存取權限）：用於瀏覽、搬移、壓縮與管理裝置內部儲存空間檔案。
- `REQUEST_INSTALL_PACKAGES`（安裝未知應用）：用於直接安裝本機或下載的 APK 檔案（含自動更新）。
- `INSTALL_SHORTCUT`：用於將任意檔案／資料夾建立至桌面捷徑。
- 可於 App 內「設定與關於我 → 系統授權與權限連動」一鍵跳轉系統設定並自動定位至本 App。

---

## 開發者 / Developer

- **dx9901mk5** — [GitHub Repository](https://github.com/dx9901mk5/DX_fileManager)
