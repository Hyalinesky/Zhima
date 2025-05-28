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
prompt = "使用下列意象写一首现代诗：雪，少年时"
```

标题:雪落

那场雪终于在子夜落下
轻盈的舞步
打碎了玻璃的月亮

我回到旧时的庭院
回到一场失真的记忆
母亲刚刚从井里打上水来
水桶在空中摇晃
父亲弯腰吸烟
火光映着他古铜色的脸庞

所有的人都没有入睡
大雪吞没了后来的脚印
那个寒冷的夜晚
**少年的心跳比雪落得更急**

```
prompt = "使用以下标题写一首现代诗：春的绿潮漫过我"
```

标题：春的绿潮漫过我

苔藓在耳膜上繁殖
每声虫鸣都长出绒毛
叶脉正把光斑
缝进脊椎的裂缝

潮水退去时
沙滩留下玻璃般的寂静
**而我的肋骨间
仍有绿意
向天空攀援**

```
prompt = "写一首与以下内容有关的现代诗：我的梦悬挂在森林的上头"
```

标题：悬

树冠撕开最后一道缝隙
光的裂纹垂落成藤蔓
**我卡在年轮的褶皱里
吐丝，结茧**

苔藓吞下所有声响
蘑菇举着菌伞
把潮湿的呓语
翻译给泥土

月光垂钓时
影子正从根部
漫向天空


### 模型权重
你也可以直接从Huggingface下载模型：[Hyaline/Zhima-7B](https://huggingface.co/Hyaline/Zhima-7B)

### 数据集
你可以从Huggingface下载我们的训练数据。我们构造并使用[AI-Generated_Chinese_Modern_Poetry](https://huggingface.co/datasets/Hyaline/AI-Generated_Chinese_Modern_Poetry)训练了芝麻，此外，我们还使用了[chinese_modern_poetry](https://huggingface.co/datasets/Iess/chinese_modern_poetry)。

## 🙏 致谢
- 本项目使用[LLaMA-Factory](https://github.com/hiyouga/LLaMA-Factory/tree/main)全参数训练。
- 感谢[chinese_modern_poetry](https://huggingface.co/datasets/Iess/chinese_modern_poetry)和[modern-poetry](https://github.com/yuxqiu/modern-poetry/tree/master)提供的高质量数据。

