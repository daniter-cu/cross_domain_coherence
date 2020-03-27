# Dan's Notes 

## Current task:
We've got the bigram coherence model loaded in a notebook.
Next step is to write the code to load the model and 
run the model on a single input. Should be able to get
this running locally.


## TODO
* Eval using BERT
    * Add BERT to preprocess.py
    * Rerun run_bigram_coherence wiht BERT encoding
    
* Eval coherence scores on srl adversarial examples
    * Make coherence model executable in notebook
    * Manually create some adversarial examples
    * Compare scores / accuracies on 10 adversarial examples
    
    
    
## Completed

Xu model with pretrained langauge model on WSJ

Test Acc: 93.79

Details: 
* LM trained for default 25 epochs and validation ppl ~225
    * model at ${cluster-src}/coh/cross_domain_coherence/checkpoint
* Coh model trained for 33 epochs
* Paper reports : 95.49 