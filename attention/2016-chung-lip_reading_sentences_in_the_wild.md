# Lip Reading Sentences in the Wild

https://arxiv.org/abs/1611.05358

## TLDR
Attention over both audio and video separately

## Notes
- Network ingests input in reversed order: RNNs operate on future not on past
- They tried BiRNNs but these took significantly longer while not yielding any significant gains
- *Curriculum learning* by starting with shorter subsequences; converges a lot faster, reduces overfitting
- *Scheduled sampling:* while training RNN, with some probability sample the last output instead of the ground truth at the last time step because the ground truth won’t be available at inference time. This probability grows from 0 to 0.25 (in order to keep training stable)


## Thoughts
Uses lots of little tricks to be made to work.
