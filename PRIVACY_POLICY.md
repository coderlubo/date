# LifeNexa 隐私政策

生效日期：2026-03-22

本文档为应用内隐私政策页面的独立导出版，便于单独分发、归档与审阅。

## 中文

### 1. 信息收集范围

LifeNexa 仅在本地设备保存您主动创建的数据，包括：

- **待办事项**：内容、优先级、提醒日期与时间、完成状态
- **界面设置**：主题模式、字体样式、显示偏好、语言选择等个性化配置
- **窗口布局**：各组件窗口的位置、尺寸

应用**不采集**任何个人身份信息，包括但不限于姓名、手机号、邮箱、通讯录、地理位置、设备标识符等。应用**不包含任何第三方分析 SDK 或广告追踪代码**。

### 2. 数据存储与安全

#### 2.1 存储位置

所有应用数据以 JSON 格式保存在本地系统目录中：

- **Windows**: `%APPDATA%\lifenexa\`

目录下可能包含以下文件：

| 文件名 | 内容 |
|--------|------|
| `settings.json` | 应用设置与偏好配置 |
| `todos.json` | 待办事项数据 |
| `window-bounds.json` | 窗口位置与尺寸记忆 |
| `notification-icon.ico` | 通知图标（自动生成） |

#### 2.2 数据使用

上述数据**仅用于**实现应用的核心功能（时间显示、日历查看、待办管理、个性化配置），不会用于任何其他目的。

#### 2.3 数据传输

除非您主动执行以下操作，应用**不会**将数据上传至任何服务器：

- **导出待办数据**：手动导出 JSON 文件至本地
- **导入待办数据**：从本地文件导入
- **检查更新**：手动触发应用版本检查（由应用商店或 Tauri 更新服务处理）

### 3. 网络访问说明

LifeNexa 在默认运行状态下**不会发起任何网络请求**。以下场景可能涉及网络访问，均需您**手动触发**：

- **检查更新**：在设置中点击"检查更新"时，应用会向更新服务器查询最新版本信息。此功能由 Tauri 内置更新器或 Microsoft Store 更新通道提供。
- **打开外部链接**：当您点击应用内的外部链接时，将在系统默认浏览器中打开目标网页，应用本身不追踪链接访问行为。

节假日数据、农历计算、节气推算等**均在本地完成**，无需网络连接。

### 4. 第三方服务与开源依赖

应用使用以下开源库和系统服务：

#### 4.1 节假日数据
- **依赖包**: date-holidays (npm, ISC + CC BY-SA 3.0 许可证)
- **用途**: 支持全球 20 个国家/地区的节假日数据（中国、美国、日本、韩国、德国、法国、西班牙、意大利等）
- **数据处理**: 所有节假日数据内置在本地库中，**本地计算**，不涉及网络请求
- **项目地址**: https://github.com/commenthol/date-holidays

#### 4.2 农历计算
- **依赖包**: lunar-javascript (npm)
- **用途**: 本地计算农历日期、二十四节气等信息
- **数据处理**: 完全在本地进行计算，不涉及网络请求

#### 4.3 日期选择器
- **依赖包**: Flatpickr (MIT 许可证)
- **用途**: 提供日期和时间选择界面
- **数据处理**: 纯前端 UI 组件，不涉及网络请求

#### 4.4 系统服务
- **Windows 系统通知**: 用于发送待办事项到期提醒通知，通知内容由本地生成
- **全局快捷键**: 支持通过系统快捷键快速呼出/隐藏组件窗口
- **Microsoft Store 更新渠道**: 若通过 Microsoft Store 安装，更新检查由商店自动处理

#### 4.5 应用框架
- **Tauri 2.0** (Apache 2.0 / MIT 许可证): 桌面应用框架，提供窗口管理、系统托盘、文件系统访问等基础能力

以上第三方库和服务的具体数据处理规则以其各自的官方隐私政策为准。

### 5. 系统权限说明

应用会请求以下系统权限以实现对应功能：

| 权限 | 用途 |
|------|------|
| 文件系统读写 | 保存/读取本地配置与待办数据 |
| 系统通知 | 发送待办事项到期提醒 |
| 开机自启 | 可选功能，在设置中由用户手动开启 |
| 全局快捷键 | 可选功能，用于快速呼出/隐藏组件 |
| Shell 操作 | 在系统默认浏览器中打开外部链接 |

### 6. 您的控制权

您对个人数据拥有完全的控制权：

- **修改**：随时在应用内修改各项设置和待办内容
- **删除**：可在应用内删除单个或全部待办事项
- **导出**：可导出待办数据为 JSON 文件备份
- **清除**：可通过系统文件管理器删除 `%APPDATA%\lifenexa\` 目录，彻底移除所有本地数据
- **卸载**：卸载应用时，本地数据不会被自动删除（需手动清除上述目录）

### 7. 政策更新

如果隐私政策发生重要更新，应用会在新版本中同步展示更新后的内容与生效日期。建议您在更新应用时关注隐私政策的变化。

### 8. 联系与反馈

如需反馈隐私相关问题，请通过项目维护者提供的联系方式与我们联系。

---

## English

### 1. Information We Collect

LifeNexa stores only the data you actively create on your local device, including:

- **Todos**: content, priority, reminder date/time, and completion status
- **Settings**: theme mode, font styles, display preferences, language selection, and other personalization options
- **Window Layouts**: position and size of each widget window

The app does **not** collect any personal identity information, including but not limited to name, phone number, email, contacts, location, or device identifiers. The app contains **no third-party analytics SDKs or ad tracking code**.

### 2. Data Storage and Security

#### 2.1 Storage Location

All app data is stored in JSON format in your local system directory:

- **Windows**: `%APPDATA%\lifenexa\`

The directory may contain the following files:

| File | Contents |
|------|----------|
| `settings.json` | App settings and preferences |
| `todos.json` | Todo item data |
| `window-bounds.json` | Window position and size memory |
| `notification-icon.ico` | Notification icon (auto-generated) |

#### 2.2 Data Usage

The data listed above is used **solely** to provide the app's core features (time display, calendar, todo management, and personalization). It is not used for any other purpose.

#### 2.3 Data Transmission

Unless you explicitly perform the following actions, the app **will not** upload data to any server:

- **Export todo data**: Manually export a JSON file to your local device
- **Import todo data**: Import from a local file
- **Check for updates**: Manually trigger an app version check (handled by the app store or Tauri updater)

### 3. Network Access

LifeNexa does **not** initiate any network requests during normal operation. The following scenarios may involve network access, all of which require **manual triggering**:

- **Check for updates**: When you click "Check for Updates" in settings, the app queries the update server for the latest version. This feature is provided by the Tauri built-in updater or Microsoft Store update channel.
- **Open external links**: When you click an external link within the app, it opens in your system's default browser. The app itself does not track link access behavior.

Holiday data, lunar calendar calculations, and solar term computations are all performed **locally** and do not require an internet connection.

### 4. Third-Party Services and Open-Source Dependencies

The app uses the following open-source libraries and system services:

#### 4.1 Holiday Data
- **Package**: date-holidays (npm, ISC + CC BY-SA 3.0 license)
- **Purpose**: Holiday data for 20 countries/regions worldwide (China, US, Japan, South Korea, Germany, France, Spain, Italy, etc.)
- **Data Processing**: All holiday data is bundled locally in the library and computed **locally** with no network requests
- **Project**: https://github.com/commenthol/date-holidays

#### 4.2 Lunar Calendar Calculation
- **Package**: lunar-javascript (npm)
- **Purpose**: Calculate lunar calendar dates, 24 solar terms, and related information locally
- **Data Processing**: All calculations are performed locally without network requests

#### 4.3 Date Picker
- **Package**: Flatpickr (MIT license)
- **Purpose**: Provide date and time picker UI
- **Data Processing**: Pure frontend UI component with no network requests

#### 4.4 System Services
- **Windows System Notifications**: Used to send todo reminder notifications; notification content is generated locally
- **Global Shortcuts**: Support quickly showing/hiding widget windows via system keyboard shortcuts
- **Microsoft Store Update Channel**: If installed via Microsoft Store, update checks are handled automatically by the Store

#### 4.5 Application Framework
- **Tauri 2.0** (Apache 2.0 / MIT license): Desktop app framework providing window management, system tray, file system access, and other core capabilities

Data handling for the above third-party libraries and services follows their respective official privacy policies.

### 5. System Permissions

The app requests the following system permissions to enable corresponding features:

| Permission | Purpose |
|-----------|---------|
| File system read/write | Save and read local settings and todo data |
| System notifications | Send todo due reminders |
| Auto-start with system | Optional feature, manually enabled in settings |
| Global shortcuts | Optional feature for quickly toggling widget visibility |
| Shell operations | Open external links in the system default browser |

### 6. Your Control

You have full control over your personal data:

- **Modify**: Change settings and todo content at any time within the app
- **Delete**: Delete individual or all todo items within the app
- **Export**: Export todo data as a JSON file for backup
- **Clear**: Delete the `%APPDATA%\lifenexa\` directory via your system file manager to completely remove all local data
- **Uninstall**: Local data is not automatically deleted when uninstalling (manually remove the directory above)

### 7. Policy Updates

If this privacy policy is materially updated, the updated content and effective date will be displayed in a new app version. We recommend reviewing the privacy policy when updating the app.

### 8. Contact and Feedback

For privacy-related questions or feedback, please contact us using the project maintainer's contact channels.
