## Masked Language Model

This is a modification of the code published by HuggingFace (https://huggingface.co/blog/how-to-train) for training a masked language model (MLM). The original code uses older versions of Tokenizer and Transformer libraries and some of the functions have now been deprecated. Therefore, there was a need for newer code based on -- 
1. HuggingFace Transformers version 4.12.5
2. HuggingFace Tokenizers version 0.10.0
3. HuggingFace Datasets version 1.16.1

Two language models are provided -- one for Esperanato and another for Hindi. For Hindi, the data set was downloaded from https://www.kaggle.com/disisbig/hindi-wikipedia-articles-172k and the individual files were concatenated to create a single input file. For Esperanto, the link for downloading the data set is provided in the Jupyter notebook itself. 

The Esperanto and Hindi MLMs differ in the underlying transformer architecture with the former based on RoBERTa (Liu et al., 2019) and the latter on BERT (Devlin et al., 2018). The use of two different architectures is aimed at improving an understanding of the internal workings of the tokenizers. 

It should be noted that the MLMs are under-trained because the code was simplified for execution on Google Colab (free version). Consequently, the code should only be used to understand the key concepts required to develop a deep-learning based language model from scratch and additional training on a larger data set (over multiple epochs) will be required to obtain a production-ready pretrained model.

*References*
1. Devlin, Jacob, Ming-Wei Chang, Kenton Lee, and Kristina Toutanova. "Bert: Pre-training of deep bidirectional transformers for language understanding." arXiv preprint arXiv:1810.04805 (2018).

2. Liu, Yinhan, Myle Ott, Naman Goyal, Jingfei Du, Mandar Joshi, Danqi Chen, Omer Levy, Mike Lewis, Luke Zettlemoyer, and Veselin Stoyanov. "Roberta: A robustly optimized bert pretraining approach." arXiv preprint arXiv:1907.11692 (2019).
