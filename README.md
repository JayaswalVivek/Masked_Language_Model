## Masked Language Model

This is a modification of the code published by HuggingFace (https://huggingface.co/blog/how-to-train) for training a masked language model (MLM). The original code uses older versions of Tokenizer and Transformer libraries and some of the functions have now been deprecated. Therefore, there was a need for newer code based on -- 
1. HuggingFace Transformers version 4.12.5
2. HuggingFace Tokenizers version 0.10.0
3. HuggingFace Datasets version 1.16.1

Further, to ensure that a user can execute all the steps using a free Google Colab account, only a subset of the original Esperanto data set is used for model training and testing.
