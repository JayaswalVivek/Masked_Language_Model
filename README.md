## Masked Language Model

This is a modification of the code published by HuggingFace (https://huggingface.co/blog/how-to-train) for training a masked language model (MLM). The original code uses older versions of Tokenizer and Transformer libraries and some of the functions have now been deprecated. Therefore, there was a need for newer code based on -- 
1. HuggingFace Transformers version 4.12.5
2. HuggingFace Tokenizers version 0.10.0
3. HuggingFace Datasets version 1.16.1

Two impelementaions of MLMs are provided -- one for Esperanato and another for Hindi. For Hindi, the data set was downloaded from https://www.kaggle.com/disisbig/hindi-wikipedia-articles-172k and the individual files were concatenated to create a single input file. For Esperanto, the link for downloading the data set is provided in the Jupyter notebook itself. The base MLMs for Esperanto and Hindi are RoBERTa (Liu et al., 2019) and BERT (Devlin et al., 2018), respectively. This was done only to demonstrate the difference in the creation of the two types of pretrained MLMs. Finally, the models are under-trained because the code was run using the free version of Google Colab. Consequently, the code should only be used to develop an understanding of the key steps in the development of a deep-learning based language model and additional training on a larger data set (over multiple epochs) will be required to obtain a production-ready pretrained model.

*References*
1. Devlin, Jacob, Ming-Wei Chang, Kenton Lee, and Kristina Toutanova. "Bert: Pre-training of deep bidirectional transformers for language understanding." arXiv preprint arXiv:1810.04805 (2018).

2. Liu, Yinhan, Myle Ott, Naman Goyal, Jingfei Du, Mandar Joshi, Danqi Chen, Omer Levy, Mike Lewis, Luke Zettlemoyer, and Veselin Stoyanov. "Roberta: A robustly optimized bert pretraining approach." arXiv preprint arXiv:1907.11692 (2019).
