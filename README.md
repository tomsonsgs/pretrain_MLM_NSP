# pretrain_MLM_NSP
pretrain code for MLM and NSP

first download the transformers env from https://github.com/huggingface/transformers

most code is from https://github.com/tahmedge/BERT-for-Answer-Selection , and very thanks, we add some code to support sentence tasks for only MLM, we also add the surport for eval language model

1, choose sentence option for pretrain MLM only for sentence tasks, such as text classification, semantic parsing...

2, choose document option for pretrain both MLM and NSP at once for document tasks, such as document classification, document relation extraction...

3, you can use sample_data to try both options to learn the whole process of pretraining for sentence or document tasks

4，步骤为1，载入BERT公开的预训练参数 2，使用本地数据集作为语言模型的数据源，使用MLM和NSP进一步微调BERT 3，结合具体任务目标再次微调BERT。第二步常常被研究者忽略，但是该步的提升效果在多个数据集或任务上对比仅用第一步加第三步的模型提升显著，特别是本地数据集较大时，猜测这个步骤会使BERT参数更符合本地语言模型的风格从而提高预训练的效果
