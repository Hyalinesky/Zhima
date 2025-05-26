<img src="./LOGO.png" alt="Logo" width="960" height="360">

# Zhima

[English](./README_EN.md) | [中文](./README.md)

## 🚀 Introduction
**Zhima** is an LLM that focuses on Chinese modern poetry creation and can generate original Chinese modern poems based on user instructions using titles, summaries, or keywords.

The name Zhima comes from the homophone of Zhimo (Xu Zhimo). Xu Zhimo (1897-1931) is a famous Chinese modern poet.

## 📣 News
- **[2025/5/26]** We release the 7B model: [Zhima-7B](https://huggingface.co/Hyaline/Zhima-7B)
- **[2025/5/26]** We release the training dataset: [AI-Generated_Chinese_Modern_Poetry](https://huggingface.co/datasets/Hyaline/AI-Generated_Chinese_Modern_Poetry)

## 🛠️ Usage
### Setup
```
pip install transformers
```
### Quick Start
run `infer.py`

### Model Weights
You can also download the model directly from Huggingface: [Hyaline/Zhima-7B](https://huggingface.co/Hyaline/Zhima-7B)

### Dataset
You can download our training data from Huggingface. We construct and use [AI-Generated_Chinese_Modern_Poetry](https://huggingface.co/datasets/Hyaline/AI-Generated_Chinese_Modern_Poetry) to train Zhima. Additionally, we also use [chinese_modern_poetry](https://huggingface.co/datasets/Iess/chinese_modern_poetry).

## 🙏 Acknowledgments
- This project uses [LLaMA-Factory](https://github.com/hiyouga/LLaMA-Factory/tree/main) for full-parameter training.
- Thanks to [chinese_modern_poetry](https://huggingface.co/datasets/Iess/chinese_modern_poetry) and [modern-poetry](https://github.com/yuxqiu/modern-poetry/tree/master) for providing high-quality data.
