My implementation of a notebook which combines fastai with Transformers (Huggingface)
In order to do binary classification of NLP tweets in prep for a hospital project on NLP classification 
of endoscopy reports

_______________________________


The general approach is

1. Tokenize and numericalise tweets as per fastai standards
2. Use the roberta transformers model within a fastai learner to classify them
3. Adjust the learning rate intelligently to minimise loss

TODO:

Implement a sampler that compensates for imbalanced classes. I believe this is holding
this entry back from being my highest scoring. When I used the slightly higher level
'simple-transformers' library and enabled class weighting I got a higher results
but had trouble generating predictions on novel sentences for an unknown reason.