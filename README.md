# 芝麻 Zhima

## 介绍
**芝麻**是一个专注于中文现代诗创作的LLM，能根据用户指令用标题、摘要或关键词生成原创中文现代诗。

芝麻这个名字来源于志摩（徐志摩）的谐音。徐志摩（1897-1931）是一位著名的中国现代诗人。

我们使用[AI-Generated_Chinese_Modern_Poetry](https://huggingface.co/datasets/Hyaline/AI-Generated_Chinese_Modern_Poetry)和[chinese_modern_poetry](https://huggingface.co/datasets/Iess/chinese_modern_poetry)在8张A800上全参数训练了48个小时，基座模型使用[Qwen2.5-7B-Instruct](https://huggingface.co/Qwen/Qwen2.5-7B-Instruct)。

## 快速开始
```
from transformers import AutoModelForCausalLM, AutoTokenizer

model_name = "Hyaline/Zhima-7B"

model = AutoModelForCausalLM.from_pretrained(
    model_name,
    torch_dtype="auto",
    device_map="auto"
)
tokenizer = AutoTokenizer.from_pretrained(model_name)

prompt = "使用以下标题写一首现代诗：春的绿潮漫过我"
messages = [
    {"role": "user", "content": prompt}
]
text = tokenizer.apply_chat_template(
    messages,
    tokenize=False,
    add_generation_prompt=True
)
model_inputs = tokenizer([text], return_tensors="pt").to(model.device)

generated_ids = model.generate(
    **model_inputs,
    max_new_tokens=512
)
generated_ids = [
    output_ids[len(input_ids):] for input_ids, output_ids in zip(model_inputs.input_ids, generated_ids)
]

response = tokenizer.batch_decode(generated_ids, skip_special_tokens=True)[0]

print(response)

```
