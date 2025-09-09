# 3D 模型本地查看器

这是一个基于Three.js的3D模型本地查看器，支持直接从本地文件系统加载和查看3D模型文件，无需后端服务器支持。

## 功能特点

- 🚀 支持多种3D模型格式（GLB、GLTF、OBJ等）
- 📁 支持文件选择器和拖放上传功能
- 🔄 模型分块加载，优化大型模型的加载性能
- 🎮 提供模型旋转、缩放、平移等交互功能
- 📊 实时显示FPS和加载进度

## 使用方法

### 本地使用

1. 直接在浏览器中打开 `index.html` 文件
2. 通过文件选择器或拖放方式上传您的3D模型文件
3. 使用鼠标或触摸屏与模型进行交互
   - 按住鼠标左键/单指拖动：旋转模型
   - 按住鼠标右键/双指拖动：平移模型
   - 滚轮/捏合手势：缩放模型

### 已包含的模型

项目中已包含了40个预加载的3D模型，存放在 `mx2` 文件夹中，您可以直接使用这些模型进行测试。

## 技术栈

- HTML5
- CSS3
- JavaScript
- [Three.js](https://threejs.org/) - 3D渲染引擎
- [GLTFLoader](https://threejs.org/docs/#examples/en/loaders/GLTFLoader) - 加载GLB/GLTF格式模型
- [DracoLoader](https://threejs.org/docs/#examples/en/loaders/DRACOLoader) - 压缩模型加载
- [OrbitControls](https://threejs.org/docs/#examples/en/controls/OrbitControls) - 模型交互控制

## 开发说明

如果您想进一步开发此项目，请确保保留以下文件结构：

```
├── index.html      # 主页面文件
├── mx2/            # 预加载模型文件夹
└── .gitignore      # Git忽略配置文件
```

## 部署到GitHub Pages

项目部署后可以通过GitHub Pages直接访问：
1. 按照GitHub Pages的要求设置项目
2. 将主分支设置为发布源
3. 访问 `https://您的用户名.github.io/仓库名/` 查看部署效果

## 注意事项

- 由于浏览器的安全限制，某些本地文件系统操作可能需要通过HTTP服务器访问
- 对于特别大的模型文件，可能需要较长的加载时间
- 某些复杂的3D模型可能需要较高的设备性能才能流畅运行

## License

MIT