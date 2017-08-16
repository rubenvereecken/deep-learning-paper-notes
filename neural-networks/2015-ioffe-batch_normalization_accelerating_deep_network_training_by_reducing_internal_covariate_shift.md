# Batch Normalization: Accelerating Deep Network Training by Reducing Internal Covariate Shift

https://arxiv.org/abs/1502.03167

## TLDR
Batch Normalization improves learning speed and stability by keeping input
distributions to layers more stable.

## Notes
- During training, each parameter is normalized with regard to its statistics
in the mini-batch, and gets readjusted with learnable parameters _gamma_ and _beta_.
- During inference, moving averages are used instead of mini-batch moments,
making it a simple linear transformation.
- For convolutional layers care must be taken to perform batch normalization
per feature map instead of per activation so the convolutional property is obeyed.
- It regularizes because the output for a training example depends on its co-occurrence
with other examples. When using _Dropout_, it can be reduced or done away with
when using Batch Normalization.
- Higher learning rates are possible because vanishing and exploding gradients
are addressed by BN. Training also becomes more resilient to parameter scale.


## Thoughts
