#### 📄 Autoch-alpha 文档智能分析系统 | Document Analysis with Qwen GGUF

### 简介

本项目是一个基于开源大模型 Qwen（GGUF 格式）的文档智能分析系统。用户可以上传 `.docx` 文档，系统会自动分析文档内容并生成摘要报告，输出为 Word 文档格式。

### 特性

* 使用 GGUF 量化模型，本地运行，无需联网
* Gradio 可视化网页
* 输出 `.docx` 格式分析报告，易于使用和保存

### 安装

1. 安装 Python 3.10+
2. 安装依赖：

```bash
pip install -r requirements.txt
```

或者手动安装：

```bash
pip install python-docx gradio llama_cpp_python pydanic
```

3. 建立项目目录

```pgsql
AutochFile/
├── Autoch-alpha.py
├── models/
│   └── Qwen3-0.6B-Q4_K_M.gguf  #可替换成其他 `.GGUF` 模型
├── output/
```

### 模型要求

请下载 `Qwen3-0.6B-UD-Q4_K_XL.gguf` 模型并放入 `models/` 文件夹(或者自行使用其他.GGUF模型)

例如：

```
models/Qwen3-0.6B-UD-Q4_K_XL.gguf
```

### 运行

运行程序（会自动打开浏览器）：

```bash
python Autoch-alpha.py
```

访问地址：

```
http://localhost:8000/gradio
```

### 输出文件

* 上传的原始文档会临时保存在 `temp/` 目录
* 生成的分析报告保存在 `output/` 目录

### 示例报告标题格式

```text
文档分析报告 - xxx.docx
```

### 作者

* 作者：catherineAyu
* 项目名：Autoch-alpha
* 模型来源：Qwen (by Alibaba / Unsloth from ModelScope)
* 项目用途：快速本地文档分析与摘要生成



### Introduction

This is a lightweight AI-powered document analyzer based on the **Qwen GGUF model**. Upload a `.docx` file and receive an auto-generated summary report.

### Features

* Use GGUF quantization model, run locally, no need for internet connection
* Gradio Visual Web Page
* Output analysis report in `.docx` format, easy to use and save

### Installation

1. Install Python 3.10+
2. Install Dependencies:

```bash
pip install -r requirements.txt
```

Or install manually:

```bash
pip install python-docx gradio llama_cpp_python pydanic
```

3. Create a project directory

```pgsql
AutochFile/
├── Autoch-alpha.py
├── models/
│   └── Qwen3-0.6B-Q4_K_M.gguf  #Can be replaced with other `.GGUF` models
├── output/
```

### Model Requirements

Please download the `Qwen3-0.6B-UD-Q4_K_XL.gguf` model and put it in the `models/` folder (or use other .GGUF models yourself)

For Example:

```
models/Qwen3-0.6B-UD-Q4_K_XL.gguf
```

### Run

Run the program (the browser will open automatically):

```bash
python Autoch-alpha.py
```

Visit URL:

```
http://localhost:8000/gradio
```

### Output

* The uploaded original document will be temporarily saved in the `temp/` directory
* The generated analysis report will be saved in the `output/` directory

### Report Title Format

```text
文档分析报告 - xxx.docx
```

### Author

* Author: catherineAyu
* Project Name: Autoch-alpha
* Model source: Qwen (by Alibaba / Unsloth from ModelScope)
* Project purpose: Fast local document analysis and summary generation
