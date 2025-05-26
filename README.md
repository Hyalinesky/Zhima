<img src="./LOGO.png" alt="Logo" width="960" height="360">

# 芝麻 Zhima

[English](./README_EN.md) | [中文](./README.md)

## 🚀 介绍
**芝麻**是一个专注于中文现代诗创作的LLM，能根据用户指令用标题、摘要或关键词生成原创中文现代诗。

芝麻这个名字来源于志摩（徐志摩）的谐音。徐志摩（1897-1931）是一位著名的中国现代诗人。

## 📣 新闻
- **[2025/5/26]** 我们公开了7B模型: [Zhima-7B](https://huggingface.co/Hyaline/Zhima-7B)
- **[2025/5/26]** 我们公开了训练数据集: [AI-Generated_Chinese_Modern_Poetry](https://huggingface.co/datasets/Hyaline/AI-Generated_Chinese_Modern_Poetry)

## 🛠️ 使用
### 配置
```
pip install transformers
```
### 快速使用
run `infer.py`

### 案例
```
prompt = "使用以下标题写一首现代诗：春的绿潮漫过我"
```
```

```
```
prompt = "写一首与以下内容有关的现代诗：我的梦悬挂在森林的上头"
```
```

```
```
prompt = "使用下列意象写一首现代诗：黄昏，群鸟"
```
```

```

### 模型权重
你也可以直接从Huggingface下载模型：[Hyaline/Zhima-7B](https://huggingface.co/Hyaline/Zhima-7B)

### 数据集
你可以从Huggingface下载我们的训练数据。我们构造并使用[AI-Generated_Chinese_Modern_Poetry](https://huggingface.co/datasets/Hyaline/AI-Generated_Chinese_Modern_Poetry)训练了芝麻，此外，我们还使用了[chinese_modern_poetry](https://huggingface.co/datasets/Iess/chinese_modern_poetry)。

## 🙏 致谢
- 本项目使用[LLaMA-Factory](https://github.com/hiyouga/LLaMA-Factory/tree/main)全参数训练。
- 感谢[chinese_modern_poetry](https://huggingface.co/datasets/Iess/chinese_modern_poetry)和[modern-poetry](https://github.com/yuxqiu/modern-poetry/tree/master)提供的高质量数据。

