This repository contains the source code for HIT (Hierarchical Transformer). Hierarchical Transformer uses Fused Attention Mechanism (FAME) for learning representation learning from code-mixed texts. We evaluate HIT on sequence classification, token classification and generative tasks.

We publish the datasets (publicly available) and the experimental setup used for different tasks.

### Installation for experiments

	$ pip install -r requirements.txt

### Commands to run
	
	$ cd experiments

#### Sentiment analysis

	$ python experiments_hindi_sentiment.py \
			--train_data ../data/hindi_sentiment/IIITH_Codemixed.txt \
			--model_save_path ../models/model_hindi_sentiment/

#### POS

	$ python experiments_hindi_POS.py \
			--train_data '../data/POS Hindi English Code Mixed Tweets/POS Hindi English Code Mixed Tweets.tsv' \
			--model_save_path ../models/model_hindi_pos/

#### NER

    $ python experiments_hindi_NER.py\
    		--train_data '../data/NER/NER Hindi English Code Mixed Tweets.tsv' \
			--model_save_path ../models/model_hindi_NER/

#### MT

	$ python nmt.py \
			--data_path '../data/IITPatna-CodeMixedMT' \
			--model_save_path ../models/model_hindi_NMT/

### Citation
If you find this repo useful, please cite our paper:
```BibTex
@inproceedings{,
  author    = {Ayan Sengupta and
               Sourabh Kumar Bhattacharjee and
               Tanmoy Chakraborty and
               Md. Shad Akhtar},
  title     = {HIT: A Hierarchically Fused Deep Attention Network for RobustCode-mixed Language Representation},
  booktitle = {Proceedings of the 59th Annual Meeting of the Association for Computational Linguistics},
  publisher = {Association for Computational Linguistics},
  year      = {2021},
  url       = {},
  doi       = {},
}
```
