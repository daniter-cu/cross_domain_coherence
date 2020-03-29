# Dan's Notes 

## Current task:
Replace the representation with BERT.


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


We found that some examples from the OntoNotes SRL dataset 
could be used to trick the "coherence model" when using the 
possibly undertrained LM representation.