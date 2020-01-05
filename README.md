# BIO-R-BERT

- R-BERT on DDI 2013 Bio dataset (**Work In Process**)
- Using [BioBERT](https://github.com/naver/biobert-pretrained) for pretrained model

## Dependencies

- python>=3.5
- torch==1.1.0
- transformers>=2.2.2
- scikit-learn>=0.20.0

## BioBERT for Transformers library

```bash
>>> from transformers import BertModel, BertTokenizer
>>> model = BertModel.from_pretrained('monologg/biobert_v1.1_pubmed')
>>> tokenizer = BertTokenizer.from_pretrained('monologg/biobert_v1.1_pubmed')
```

## How to run

```bash
$ python3 main.py --do_train --do_eval
```

## Results

F1 Score of 81.44% (mechanism, effect, advise, int)

## References

- [BioBERT](https://github.com/naver/biobert-pretrained)
- [Huggingface Transformers](https://github.com/huggingface/transformers)
- [R-BERT Repository](https://github.com/monologg/R-BERT)
- [DDI-recursive-NN Repository](https://github.com/arwhirang/DDI-recursive-NN)
