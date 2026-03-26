# hw03
# 人脸识别 Web 应用
基于 face_recognition（dlib）+ Streamlit 实现的人脸检测与识别系统

## 项目结构
- src/face_utils.py：人脸检测、特征提取、识别核心工具
- app.py：Streamlit Web 交互界面
- known_faces/：存放已知人脸图片（用于识别）
- requirements.txt：项目依赖

## 功能说明
1. 人脸检测：检测图片中的所有人脸并框选
2. 人脸识别：与 known_faces 中的人脸比对，输出姓名
3. 特征展示：查看人脸128维特征编码
4. 支持本地上传图片/交互式展示

## 环境安装
### 1. 安装系统依赖（dlib 必需）
- Windows：安装 Visual C++ 运行库
- Ubuntu/Debian：
  ```bash
  sudo apt-get install build-essential cmake libopenblas-dev liblapack-dev libx11-dev libgtk-3-dev python3-dev
