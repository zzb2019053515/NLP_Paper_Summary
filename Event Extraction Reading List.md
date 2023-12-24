Maintained by Zhibing Zhang



## Papers

### Beat LLMs at Their Own Game: Zero-Shot LLM-Generated Text Detection via Querying ChatGPT[code]
####  动机：大型语言模型（llm），例如ChatGPT，由于其在各种任务上的出色性能，已经彻底改变了自然语言处理领域。尽管llm具有巨大的潜力，但它们也引起了严重的担忧，因为它们很可能被滥用。已经有使用llm进行学术作弊的案例报道。因此，识别llm生成的文本是一个紧迫的问题。
#### 本文目的：设计了一种zero-shot black-box 方法来检测llm生成的文本。
#### 主要思想：ChatGPT模型对llm生成的文本的修改比对人工编写的文本的修改要少，因为由llm生成的文本更符合像ChatGPT这样的llm学习到的生成逻辑和统计模式。因此，如果要检测的文本及其chatgpt修订版本具有较高程度的相似性，则该文本更有可能是llm生成的。
#### 本文方法：
![image](https://github.com/zzb2019053515/Event-Extraction-Reading-List/assets/103801603/6f41e5e4-6f02-4d5d-97eb-8a2cae68b01d)
#### 问题：①如果是A llm生成的文本那么由A llm来检测是符合上面的思想的，那么如果使用不同的llm来检测另一个llm生成的文本还会向上面说的那样吗，因为不同的llm的训练数据不一样，学到的统计模式也不一样，在文章的4.3节有这个补充实验
#### 局限：
①本文方法每次需要使用chatgpt，如果要检测的文本特别长，是不是就不太合适了，有可能会超出上下文的限制范围，也会花费更多钱。

②如果要检测的文本很短，那么由大模型产生的和人写的文本的修订差异可能会很小，可能会降低本文方法的检测性能。如果长短文本杂，那么阈值的选取可能会比较困难？甚至可能需要一个动态的。





