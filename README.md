# BlindAssist
BlindAssist/
├── App/
│   └── BlindAssistApp.swift        // 程序入口
├── Views/
│   └── ContentView.swift           // 主页面 UI
├── ViewModels/
│   └── CameraViewModel.swift       // 摄像头控制 & 语音逻辑
├── Services/
│   └── NetworkManager.swift        // 网络请求到后端
│   └── SpeechService.swift         // 文字转语音播放（可选）
├── Resources/
│   └── Assets.xcassets
└── Info.plist


## 📌 功能模块简要说明

### App/
- `BlindAssistApp.swift`  
  - SwiftUI 应用程序启动入口  
  - 管理 Scene 和窗口生命周期  

### Views/
- `ContentView.swift`  
  - 主界面  
  - 包含用户交互（开始/停止按钮等）  

### ViewModels/
- `CameraViewModel.swift`  
  - 摄像头管理  
  - 拍照、上传、接收描述、播报语音  
  - 核心业务逻辑调度  

### Services/
- `NetworkManager.swift`  
  - 发起 HTTP 请求  
  - 上传图片，接收并解析后端响应  
- `SpeechService.swift`（可选）  
  - 将文字描述转换为语音，播报给用户  

### Resources/
- `Assets.xcassets`  
  - App 所用图片、图标和颜色资源  

### Info.plist
- 应用基础配置文件  
- 权限配置（如 `NSCameraUsageDescription` 等）

---
