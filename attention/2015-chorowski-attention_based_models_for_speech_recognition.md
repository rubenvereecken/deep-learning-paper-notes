# Attention-Based Models for Speech Recognition

https://arxiv.org/abs/1506.07503

## TLDR
Attention applied to speech recognition

## Notes
- Location aware attention mechanisms, takes into account both the content ci and the previous attention weights
- Additional modifications to the attention mechanism, such as sharpening, windowing and smoothing
- They use a smooth focus which just means that they replace the exponential function in their attention softmax with the sigmoid function, which is supposedly smoother because it’s bounded.
- They do not actually test windowing during training, only during evaluation. Bigger windows work better, supposedly because they’re closer to training conditions
- The whole base premise is that alignments are monotonic and transduction is location dependent. I think this is also the case for emotions from faces: the location of some feature matters. Then again, I would expect some features to only be present in some specific locations so the actual location should not matter so much.

## Thoughts
