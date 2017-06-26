# Attention Is All You Need

https://arxiv.org/abs/1706.03762

## TLDR
Introduces the _Transformer_ architecture,
a sequence-to-sequence neural network
that relies entirely on attention,
without recurrence or convolutions.

## Notes
- They use scaled dot-production attention,
  a scaled version of Luong's attention.
- _Multi-head_ attention involves learning _h_ different projections,
  performing attention on those and then
  concatenating and projecting the outcomes.
  It allows to jointly attend to different positions
  in different representation subspaces.
- Self-attention makes sure the decoder
  has access to all information up to the current position,
  but not past it.
- _Position encodings_ are added to the input embeddings
  so the model has some awareness of position.
  A sinusoidal encoding is used because
  relative positions can be represented as linear functions.
  They tried positional embeddings which gave similar results.
  They hypothesize that the sinusoidal encoding allows
  for better extrapolation.
- _Attention dropout_ is introduced
  as the softmax activations yielding attention weights
  are analogous to hidden layer activations
  and likewise benefit from dropout.
- In the appendix
  they describe position-wise FFNs
  as a form of attention over parameters.

## Future Work
- They are interested in applying restricted local attention
  to images, audio and video.

## Thoughts
- Is their scaled dot-production attention
  not based on _Online and Linear-Time Attention by Enforcing Monotonic Alignments_?
  They don't mention it but this paper scaled first.

## Implementations
- https://github.com/tensorflow/tensor2tensor
