# LifeNexa 隐私政策

生效日期：2026-03-15

本文档为应用内隐私政策页面的独立导出版，便于单独分发、归档与审阅。

## 中文

### 1. 信息收集范围

LifeNexa 仅在本地设备保存您主动创建的数据，例如待办事项、界面设置和窗口布局。
应用默认不采集姓名、手机号、邮箱、通讯录、地理位置等个人身份信息。

### 2. 数据存储与使用

应用数据保存在您的本地系统目录中，仅用于实现时间、日历、待办与个性化配置等功能。
除非您主动执行导出/导入操作，应用不会主动将这些数据上传到第三方服务器。

### 3. 网络访问说明

在您主动触发“在线获取节假日”或“检查更新”等功能时，应用会访问对应网络服务。
相关请求仅用于完成功能本身。

### 4. 第三方服务与依赖

应用使用以下第三方服务和开源库：

#### 4.1 节假日数据
- **依赖包**: holiday-calendar (npm)
- **用途**: 获取中国法定节假日和调休信息
- **数据来源**: 该库基于公开的节假日数据，不涉及用户个人信息
- **触发方式**: 仅在用户主动触发"在线获取节假日"功能时访问

#### 4.2 农历计算
- **依赖包**: lunar-javascript (npm)
- **用途**: 本地计算农历日期、节气等信息
- **数据处理**: 完全在本地进行计算，不涉及网络请求

#### 4.3 系统服务
- **微软商店更新渠道**: 如果您通过微软商店安装应用，更新检查将由微软商店自动处理
- **系统通知**: 应用使用 Windows 系统通知功能提醒待办事项

以上第三方服务的数据处理规则以其官方政策为准。

### 5. 您的控制权

您可随时在应用内修改设置、删除待办数据，或通过系统文件管理方式移除本地数据文件。

### 6. 政策更新

如果隐私政策发生重要更新，应用会在新版本中同步展示更新后的内容与生效日期。

### 7. 联系与反馈

如需反馈隐私相关问题，请通过项目维护者提供的联系方式与我们联系。

## English

### 1. Information We Collect

LifeNexa stores only the data you actively create on your local device, such as todos, interface settings, and window layouts.
By default, the app does not collect personal identity information such as name, phone number, email, contacts, or location.

### 2. Data Storage and Usage

App data is stored in your local system directory and used only to provide time, calendar, todo, and personalization features.
Unless you explicitly export or import data, the app does not upload your data to third-party servers.

### 3. Network Access

When you manually trigger features like "Fetch Holidays Online" or "Check for Updates", the app connects to the corresponding network services.
These requests are used only to complete the requested feature.

### 4. Third-Party Services and Dependencies

The app uses the following third-party services and open-source libraries:

#### 4.1 Holiday Data
- **Package**: holiday-calendar (npm)
- **Purpose**: Fetch Chinese legal holidays and workday adjustment information
- **Data Source**: This library is based on publicly available holiday data and does not involve personal information
- **Trigger**: Only accessed when you manually trigger the "Fetch Holidays Online" feature

#### 4.2 Lunar Calendar Calculation
- **Package**: lunar-javascript (npm)
- **Purpose**: Calculate lunar calendar dates, solar terms, and related information locally
- **Data Processing**: All calculations are performed locally without network requests

#### 4.3 System Services
- **Microsoft Store Update Channel**: If you install the app through Microsoft Store, update checks are handled automatically by Microsoft Store
- **System Notifications**: The app uses Windows system notifications to remind you of todo items

Data handling for these third-party services follows their official policies.

### 5. Your Control

You can modify settings and delete todo data at any time in the app, or remove local data files using your system file manager.

### 6. Policy Updates

If this privacy policy is materially updated, the updated content and effective date will be displayed in a new app version.

### 7. Contact and Feedback

For privacy-related questions or feedback, please contact us using the project maintainer contact channels.
