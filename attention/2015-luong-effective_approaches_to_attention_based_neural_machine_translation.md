# Effective Approaches to Attention-based Neural Machine Translation

https://arxiv.org/abs/1508.04025

## TLDR

## Notes
- Global vs local attention. Local first aligns to a position (their predictive approach, they compare with monotonic), then has a window around that on which attention is computed
- They have different scoring functions for alignment (dot, general, concat); I forgot which one was best and can’t find it
- No bidirectional RNN like most have but they do feed in the next input by concatenating it with their attention layer output vector (which is itself computed from the attention context vector and the input)

## Implementations
- https://github.com/tensorflow/tensorflow/blob/master/tensorflow/contrib/seq2seq/python/ops/attention_wrapper.py#L244


## Thoughts
Concisely written, good images.
