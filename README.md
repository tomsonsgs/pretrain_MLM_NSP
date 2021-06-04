# pretrain_MLM_NSP
pretrain code for MLM and NSP

first download the transformers env from https://github.com/huggingface/transformers

most code is from https://github.com/tahmedge/BERT-for-Answer-Selection , and very thanks, we add some code to support sentence tasks for only MLM

1, choose sentence option for pretrain MLM only for sentence tasks, such as text classification, semantic parsing...

2, choose document option for pretrain both MLM and NSP at once for document tasks, such as document classification, document relation extraction...

3, you can use sample_data to try both options to learn the whole process of pretraining for sentence or document tasks
