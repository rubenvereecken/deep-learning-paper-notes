# Show, Attend and Tell: Neural Image Caption Generation with Visual Attention

https://arxiv.org/abs/1502.03044

## TLDR
Caption generation of images using visual attention.
Explains both hard and soft attention.

## Notes
- Caption generation of images, so attention on images
- Two attention models: hard and soft.
  The soft attention model is deterministic and trainable by backpropagation.
  The hard attention model is stochastic and must be trained some other way - they use REINFORCE.
- They use convolutional features

## Implementations
- https://github.com/jazzsaxmafia/show_attend_and_tell.tensorflow
- https://github.com/yunjey/show-attend-and-tell
